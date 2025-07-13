# 🧹 Clear The Clutter

This project organizes files in a given directory by sorting them into folders based on their file extensions. It helps in cleaning up cluttered folders by automatically grouping similar file types.

---

## 📁 Features

- 📂 Automatically detects and organizes files by extension
- 🧠 Ignores `.js` and `.json` files
- 📦 Creates new folders for each unique extension if not already present
- 🔄 Moves files to their respective folders

---

## 🛠️ Tech Stack

- **Node.js**
- **fs/promises** & **fs** modules
- **path** module

---

## 📂 How It Works

1. Reads all files in the target directory.
2. For each file:
   - Skips `.js` and `.json` files.
   - Checks the file extension.
   - If a folder with the extension name exists, moves the file there.
   - If not, creates the folder and then moves the file.

---

## 🧪 Usage

### 1. Clone the repository or copy the script

### 2. Modify the `basepath` variable in the script to point to your target folder:
```js
const basepath = "C:\\path\\to\\your\\directory"
```

### 3. Run the script:
```bash
node index.js
```

---

## 🔐 Example

If your folder contains:
```
photo.jpg
document.pdf
script.js
notes.txt
```

After running the script:
```
📁 jpg
    └── photo.jpg
📁 pdf
    └── document.pdf
📁 txt
    └── notes.txt
script.js
```

`.js` and `.json` files remain in the root directory.

---

## 👨‍💻 Author

- **Your Name**
- [GitHub](https://github.com/your-username)

---

## 📄 License

This project is licensed under the **ISC License**.
