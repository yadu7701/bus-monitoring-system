Got it 👍 You want your entire project description **converted into a clean GitHub-style README** with headings, bullet points, and code blocks.

Here’s your content transformed properly:

```markdown
# 🚌 Bus Entry-Exit Logging System (RFID + Flask)

This project is a Flask-based web application that logs the entry and exit times of buses using RFID tags and stores the data in an Excel file (`buslog22.xlsx`).  
The system reads data from a serial-connected RFID reader (e.g., Arduino), automatically toggles the bus status (**Entered/Exited**), and provides a user interface for administration.

---

## 🔧 Features
- 📟 Real-time data logging via serial port (**COM3**).
- 🕒 Timestamped log entries of bus movement (**entry/exit**).
- 🧾 Excel file generation for all activity (`buslog22.xlsx`).
- 🌐 Flask-based UI to view and manage RFID tags.
- 📥 Downloadable logs through `/download`.
- ➕ Add new RFID UIDs to the system.
- 🔁 Status toggling logic based on last recorded action.

---

## 📁 Project Structure
```

├── app.py              # Main Flask application
├── buslog22.xlsx       # Excel log file (generated)
├── rfid\_tags.json      # Stores UID to bus number mapping
├── templates/
│   └── admin.html      # Admin interface

````

---

## 🚀 Getting Started

### ✅ Prerequisites
- Python 3.x  
- Flask  
- Pandas  
- PySerial  

### 📦 Install Dependencies
```bash
pip install flask pandas pyserial
````

### 🔌 Connect RFID Reader

Ensure your RFID reader (via Arduino or similar) is connected to **COM3**.
Update COM3 in the script if needed.

---

## 🔌 Endpoints

| Endpoint    | Description                          |
| ----------- | ------------------------------------ |
| `/`         | Admin panel showing UID-bus mappings |
| `/download` | Download the Excel log file          |
| `/add-uid`  | POST route to add a new UID + name   |
| `/get-data` | Returns JSON of current bus events   |

---

## 🧠 Logic Overview

* **Serial Reader Thread** → Reads RFID tag from Arduino via COM3.
* **Toggle System** → First scan = *Entered*, next = *Exited* (and so on).
* **Log Storage** → Every event is saved with timestamp and status.
* **Web Interface** → Admin can add UID-bus mappings and download logs.

---

## 📌 Note

Ensure your Arduino is programmed to send messages like:

```
Access granted for: Bus42
```

The status alternates based on the last recorded action for a bus.

---

## 📜 License

This project is open-source. Feel free to modify and improve.

```

---

👉 Would you like me to also **add shields.io badges** (Python, Flask, License, etc.) at the top to make it look even more professional for GitHub?
```
