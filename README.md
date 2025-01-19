# 📧 OM's Mail Application - README

Welcome to Sagar's Mail Application! This is a simple GUI-based email-sending application built using Python and the Tkinter library. This application allows users to send emails conveniently via Gmail's SMTP server.

---

## 🌟 Features

- **User-Friendly Interface**: Easy-to-use GUI for composing and sending emails.
- **Secure**: Uses Gmail's secure SMTP with TLS.
- **Customizable**: Enter the sender email, recipient email, subject, and body.

---

## 📋 Prerequisites

### Before you start, ensure you have the following:

1. **Python Installed**: Python 3.6 or higher.
2. **Gmail Account**:
   - Make sure to enable "Allow less secure apps" in your Gmail settings, or create an **App Password** if you have two-factor authentication enabled.
3. **Libraries**: Install the required Python libraries:
   - `tkinter` (standard with Python)
   - `smtplib` (standard with Python)

---

## 🚀 How to Run

1. Save the provided code into a file, e.g., `mail_app.py`.
2. Open a terminal or command prompt in the directory where the file is saved.
3. Run the script with the command:
   ```bash
   python mail_app.py
   ```
4. The application window will open. Fill in the following fields:
   - **From**: Your Gmail address.
   - **App Password**: The app password generated from your Gmail account.
   - **To**: Recipient’s email address.
   - **Subject**: Subject of the email.
   - **Body**: Email content.
5. Click the **Send** button to send the email.

---

## 🛠️ Code Overview

### Class: `MailApp`
This class handles all the functionality of the mail application, including the UI and SMTP communication.

#### Components:
1. **UI Elements**:
   - `Label` and `Entry` for fields: From, App Password, To, Subject.
   - `Text` widget for the email body.
   - `Button` to trigger email sending.

2. **SMTP Communication**:
   - Uses `smtplib.SMTP` to connect to Gmail's SMTP server (`smtp.gmail.com`) on port 587.
   - Authenticates using the provided email and app password.
   - Sends the composed email to the specified recipient.

3. **Error Handling**:
   - Displays an error message if authentication fails (e.g., invalid credentials).

---

## 🧩 Error Handling

- **Authentication Error**:
  If you enter incorrect email credentials, the app will show a pop-up message with the error "Invalid email address or app password." Please double-check your Gmail address and app password.

---

## 📌 Notes

- This application is designed for **educational purposes**. For production use, consider additional security measures, such as using encrypted storage for sensitive information.
- Gmail may restrict access due to unusual activity. Check your Gmail settings or inbox for security alerts if you face issues.

---

## 📜 License
This project is released under the MIT License. Feel free to modify and use it as per your needs.

---

Thank you for using OM's Mail Application! 😊📨

