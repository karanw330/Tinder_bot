# 🚀 Tinder Auto Disliker Bot

This is a Python-based automation bot for Tinder that logs in via Facebook and automatically dislikes profiles.  
It uses **Selenium** to interact with Tinder's web interface and simulates manual user actions.

---

## 📌 Features

- Automates Tinder login via **Facebook authentication**.
- Handles popups like **location permissions**, **notifications**, and **cookie consent** (as of May 2025).
- Automatically dislikes profiles (can be configured to like as well).
- Configurable number of profiles to swipe left (NOPE).
- Bypasses occasional popups that block swipes.

---

## 🛠 Technologies Used

- **Python 3.8+**
- **Selenium**
- **ChromeDriver**
- **Tinder Web**
- **Facebook Login Integration**

---

## ✅ Prerequisites

- Python 3.8+
- Google Chrome installed
- ChromeDriver installed (version must match your Chrome browser)
- A **Tinder account linked with Facebook**

---

## 📦 Installation

1. Install dependencies:
```bash
pip install selenium
```

---

## Configuration
- Replace the placeholders in the script:
-- fb_email.send_keys("EMAIL") Replace with your Facebook email
-- fb_pass.send_keys("PASSWORD")  # Replace with your Facebook password

- Optionally, you can modify: for n in range(100): to control how many profiles the bot will attempt to dislike.

---

## 🔄 Optional: Liking Profiles Instead of Disliking
- To like profiles instead of disliking, replace this section:
- **if button.text == "NOPE": button.click()** with **if button.text == "LIKE": button.click()**

## ⚠️ Important Notes
- ChromeDriver must match your Chrome version.
- Tinder frequently updates its site structure, which can break XPaths or selectors in the script.
- Automating Tinder violates their Terms of Service. This is made purely as a personal project.
- **Don't be a creep. Be a Coder**
