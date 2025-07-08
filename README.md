# safeiofile 📂 — Safe & Simple File Operations in Python

`safeiofile` is a minimal, cross-platform Python library designed to simplify and secure common file operations like reading, writing, appending, backing up, and log rotation.

---

## 🚨 The Problem

Working with files in Python using built-in methods like `open()` can be:

- Verbose and repetitive
- Prone to human error (e.g., forgetting to close files)
- Lacking in safety features like auto-backups or size checks
- Inflexible for chaining operations or automating logs

While Python provides powerful tools, it misses a lightweight abstraction for **everyday file tasks** with added safety and clarity.

---

## ✅ The Solution: `safeiofile`

`safeiofile` wraps Python’s file handling into a clean, chainable interface with built-in safety features:

- ✔️ Simple `.read()`, `.write()`, `.append()` methods
- 🔁 Auto-rotates large files to avoid crashes or memory issues
- 🛡️ Built-in `.backup()` with timestamped copies
- 🧠 Fluent, chainable syntax (`.write().append().backup()`)

---

## 📦 Installation

```bash
pip install safeiofile
```

---

## 🔧 Features

- ✅ `read()` – Reads and returns the content of the file
- ✅ `write(data)` – Writes data to the file, replacing existing content
- ✅ `append(data)` – Appends a line of data with newline to the file
- ✅ `backup()` – Creates a timestamped `.bak` backup copy of the file
- ✅ `rotate_if_large(max_mb=1)` – If file size > max_mb, creates a backup and clears the original
- ✅ Chainable API – Write, append, backup, and rotate in a single line

---

## 📚 License

This project is licensed under the **MIT License** – do anything you want, but give credit and don't hold the author liable.

---

## 🌐 Project Links

- 🔗 GitHub: [https://github.com/omakr086/safeio_Lib](https://github.com/omkar086/safeiofile_Lib)
- 📦 PyPI: [https://pypi.org/project/safeio](https://pypi.org/project/safeiofile)

