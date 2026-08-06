# DUAL-SECURITY-BANK-LOCKER
# 🔐 Dual Security Bank Locker using LPC2148 (ARM7)

<p align="center">
  <img src="Images/bank_locker_banner.jpg" width="850">
</p>

<p align="center">

**Embedded Security System using ARM7 LPC2148 with Password and Fingerprint Authentication**

</p>

---

# 📖 Project Description

The **Dual Security Bank Locker using LPC2148 (ARM7)** is an embedded security system designed to provide enhanced protection for bank lockers through **two-factor authentication**. The system combines **password verification** and **biometric fingerprint authentication**, ensuring that only authorized users can access the locker.

The **LPC2148 ARM7 Microcontroller** acts as the main controller of the system. Initially, the user enters a password using the **4×4 Matrix Keypad**. After successful password verification, the system requests fingerprint authentication through the **R305 Fingerprint Sensor**. If both authentication stages are successful, the controller activates the relay to unlock the locker. Otherwise, access is denied, the locker remains locked, and the buzzer generates an alert.

This project demonstrates the practical implementation of **embedded systems, ARM7 microcontrollers, biometric security, UART communication, LCD interfacing, keypad scanning, and relay control** for secure banking and industrial applications.

---

# 📸 Project Preview

<table align="center">

<tr>

<td align="center">

<img src="Images/lpc2148_board.jpg" width="320"><br>

### 🧠 LPC2148 ARM7 Development Board

The LPC2148 development board serves as the central controller of the project. It manages password verification, fingerprint communication, LCD display, relay control, and security alerts.

</td>

<td align="center">

<img src="Images/bank_locker.jpg" width="320"><br>

### 🔐 Dual Security Bank Locker

Illustration of the dual authentication bank locker where users authenticate using a password and fingerprint before gaining access.

</td>

</tr>

</table>

---

# 🎯 Aim

To design and implement a **Dual Security Bank Locker System using LPC2148 ARM7 Microcontroller** that provides secure access using **password authentication** and **fingerprint verification**, preventing unauthorized access to bank lockers.

---

# ✨ Features

- 🔐 Dual-Level Authentication (Password + Fingerprint)
- 🖐️ Biometric Fingerprint Verification
- 🔢 Password Entry using 4×4 Matrix Keypad
- 📺 16×2 LCD Status Display
- 🔒 Relay Controlled Electronic Locker
- 🚨 Unauthorized Access Alarm using Buzzer
- ⚡ Fast Real-Time Embedded Operation
- 🧠 LPC2148 ARM7 Based Design
- 🔋 Low Power Embedded System

---

# 🛠️ Hardware Components

<table align="center">

<tr>

<td align="center">

<img src="Images/keypad.jpg" width="220"><br>

### 🔢 4×4 Matrix Keypad

Used to enter the password before fingerprint authentication.

</td>

<td align="center">

<img src="Images/fingerprint_sensor.jpg" width="220"><br>

### 🖐️ R305 Fingerprint Sensor

Captures and verifies the user's fingerprint using UART communication.

</td>

</tr>

<tr>

<td align="center">

<img src="Images/lcd.jpg" width="240"><br>

### 📺 16×2 LCD Display

Displays authentication status such as:

• Enter Password

• Scan Finger

• Access Granted

• Access Denied

</td>

<td align="center">

<img src="Images/lpc2148_board2.jpg" width="240"><br>

### 🧠 LPC2148 ARM7 Board

Interfaces with keypad, fingerprint sensor, LCD, relay, and buzzer.

</td>

</tr>

</table>

---

# 💻 Software Requirements

| Software | Purpose |
|-----------|---------|
| Keil µVision IDE | Embedded C Development |
| Embedded C | Firmware Programming |
| Flash Magic | Program Uploading |
| Proteus | Circuit Simulation |
| Git | Version Control |
| GitHub | Project Repository |

---

# 🏗️ System Architecture

```text
           +-------------------+
           | 4×4 Matrix Keypad |
           +---------+---------+
                     |
                     |
        +------------v-------------+
        |                          |
        |     LPC2148 ARM7 MCU     |
        |                          |
        +------+---------+---------+
               |         |
               |         |
     +---------v-+   +---v----------------+
     | 16×2 LCD  |   | Fingerprint Sensor |
     +-----------+   +--------------------+
               |
               |
       +-------v------+
       | Relay Module |
       +-------+------+
               |
         Electronic Lock
               |
          Bank Locker Door

               |
          +----v----+
          | Buzzer  |
          +---------+
```

---

# ⚙️ Working Principle

1. Power ON the system.
2. LCD displays **Enter Password**.
3. User enters password using the keypad.
4. LPC2148 verifies the password.
5. If the password is correct, LCD displays **Scan Fingerprint**.
6. User places a finger on the R305 fingerprint sensor.
7. The fingerprint module compares the fingerprint with the stored template.
8. If the fingerprint matches:
   - Relay is activated.
   - Electronic locker unlocks.
   - LCD displays **Access Granted**.
9. If either the password or fingerprint is incorrect:
   - Locker remains locked.
   - LCD displays **Access Denied**.
   - Buzzer generates an alarm.

---

# 📸 System Demonstration

<table align="center">

<tr>

<td align="center">

<img src="Images/fingerprint_demo.jpg" width="320"><br>

### 🖐️ Fingerprint Authentication

</td>

<td align="center">

<img src="Images/bank_locker.jpg" width="320"><br>

### 🔐 Locker Authentication

</td>

</tr>

</table>

---

# 📊 Output

### ✅ Successful Authentication

- Password Verified
- Fingerprint Matched
- Relay Activated
- Locker Opened
- LCD Displays **Access Granted**

### ❌ Failed Authentication

- Wrong Password
- Invalid Fingerprint
- Locker Remains Locked
- LCD Displays **Access Denied**
- Buzzer Activated

---

# 🌍 Applications

- 🏦 Bank Locker Security
- 🏠 Home Security Systems
- 🏢 Office Access Control
- 🏥 Hospital Equipment Security
- 🔐 Personal Locker Systems
- 🏭 Industrial Security

---

# 🔮 Future Enhancements

- ☁️ IoT Based Locker Monitoring
- 📱 Mobile Application Control
- 📩 SMS & Email Alerts
- 📷 Face Recognition
- 🔒 AES Encrypted Authentication
- 🌐 Cloud Database Integration

---

# ✅ Conclusion

The **Dual Security Bank Locker using LPC2148 (ARM7)** provides a secure and reliable authentication mechanism by combining password verification with biometric fingerprint authentication. The system enhances security compared to traditional locker systems and demonstrates the application of ARM7-based embedded systems in modern access control solutions.

---

# 👨‍💻 Author

**MANNEM Jashuva**

**B.Tech Graduate**

**Electronics and Communication Engineering (ECE)**

**Project Title:** Dual Security Bank Locker using LPC2148 (ARM7)

---

# 📜 License

This project is developed for educational and demonstration purposes only.
