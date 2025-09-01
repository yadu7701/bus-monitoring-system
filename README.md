# bus-monitoring-system
This project is a Flask-based web application that logs the entry and exit times of buses using RFID tags and stores the data in an Excel file (buslog22.xlsx). The system reads data from a serial-connected RFID reader (e.g., Arduino), automatically toggles the bus status (Entered/Exited), and provides a user interface for administration

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
