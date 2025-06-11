
# CobaltScreenTime

**CobaltScreenTime** is a Windows utility for managing and restricting computer usage time.  
It provides flexible scheduling options to help enforce healthy screen time limits, especially for shared or family computers.

---

## ✨ Features

- ⏰ **Login Restriction by Time Range**  
  Prevents login to a specific user account during defined hours.  
  > Users already logged in will **not be forcibly logged out**.

- 🔁 **Scheduled Automatic Restart**  
  Restarts the computer daily at a specified time, useful for enforcing logout during restricted periods.

- 💬 **Optional Warning Message**  
  Displays a custom message before the scheduled restart, giving the user time to save their work.

---

## ⚙️ Installation

1. Clone the repository or download the latest release.
2. Make sure you have Python 3.8+ installed.
3. Install required dependencies (if any):
   ```bash
   pip install -r requirements.txt
   ```
4. Run the script with administrative privileges:
   ```bash
   python cobalt_screentime.py
   ```

---

## 🧩 Usage Example

To block user access from **01:00 AM to 06:00 AM**, and ensure they are logged out:

1. Set login restriction for the desired user between `01:00`–`06:00`.
2. Set a scheduled reboot at `01:00`.
3. (Optional) Enable a warning message to be displayed at `00:55`.

> ⚠️ The login restriction **only blocks new logins** — it doesn't affect users already signed in.  
> To enforce logout, combine it with the reboot feature.

---

## 🔐 Important Notes

- Be careful when applying login restrictions to **administrator accounts**.  
  If blocked, you won’t be able to log in — even with the correct password.

- After a reboot, the login restriction applies immediately based on the configured schedule.

- Use responsibly. This tool is intended for **local** time-management enforcement and is not a security feature.

---

## 📁 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

## 🧠 Inspiration

Created as a lightweight tool to assist with screen time limitations at the operating system level, without the need for third-party monitoring or background services.

---

## 📞 Support

For questions, suggestions or bug reports, please open an issue in the [GitHub repository](https://github.com/your-username/CobaltScreenTime).
