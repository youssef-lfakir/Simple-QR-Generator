# Python QR Code Generator

## 📌 About The Project
This is a fast and efficient Python script designed to generate QR codes from any URL, text, or data string. I built this project to practice Python scripting, understand how external libraries work, and automate simple tasks. It is a great starting point for understanding data encoding in Python.

## ✨ Features
* **Fast Generation:** Creates a QR code in milliseconds (j-joz2 mn t-taniya).
* **Customizable:** You can easily change the link or text inside the code.
* **Offline Work:** Generates the image locally without needing an internet connection.

## ⚙️ Prerequisites & Installation
Before you run the script, you need to install the required library. Open your Terminal or Command Prompt and run this command:
`pip install qrcode[pil]`

## 🛠️ Built With
* **Language:** Python 3.x
* **Library:** `qrcode` (A popular Python image library for generating QR codes)

## 🚀 How It Works
1. **Input:** The script takes a specific URL (like a Spotify profile, Instagram link, or personal website).
2. **Processing:** It uses the `qrcode` library to encode the data into a 2D matrix (the QR code pattern).
3. **Output:** The generated QR code is automatically saved as an image file (for example, `insta_qr.png`) in your current project folder.

## 💻 Code Example
```python
import qrcode 

# 1. Add your URL or text here
data = "[https://open.spotify.com/intl-ar/track/1chsFxuRdocgGwhhCYfZ9m?si=53157e3c8e554fcc](https://open.spotify.com/intl-ar/track/1chsFxuRdocgGwhhCYfZ9m?si=53157e3c8e554fcc)"

# 2. Generate the QR Code
q = qrcode.make(data)

# 3. Save it as an image file
q.save("insta_qr.png")

print("QR Code generated successfully!")
