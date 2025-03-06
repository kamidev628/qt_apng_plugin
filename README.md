# 🎨 Qt APNG Plugin  

🖼 **A Qt plugin for Animated PNG (APNG) support**, enabling seamless animation rendering in Qt applications!  

![Qt](https://img.shields.io/badge/Qt-6-green) ![C++](https://img.shields.io/badge/Language-C++-blue) ![APNG](https://img.shields.io/badge/Format-APNG-orange)  
![GitHub stars](https://img.shields.io/github/stars/kamidev628/qt_apng_plugin?style=social) ![GitHub forks](https://img.shields.io/github/forks/kamidev628/qt_apng_plugin?style=social)  

---

## ✨ Features  

✅ **APNG (Animated PNG) support** – Load and display APNG files in Qt  
✅ **Seamless Integration** – Works as a Qt image plugin (`QImageIOPlugin`)  
✅ **Efficient Rendering** – Optimized for performance  
✅ **Cross-Platform** – Works on Windows, macOS, and Linux  

---

## 🚀 Installation & Build  

### 1️⃣ Prerequisites  
Ensure you have:  
- **Qt 6+** installed  
- A **C++ compiler** (GCC, MSVC, Clang, etc.)  
- **CMake**  

### 2️⃣ Clone & Build  
```sh
git clone https://github.com/kamidev628/qt_apng_plugin.git
cd qt_apng_plugin
mkdir build && cd build
cmake ..
make
```

### 3️⃣ Install the Plugin  
Move the compiled plugin to your Qt plugins directory:  
```sh
cp libqapng.so /path/to/Qt/plugins/imageformats/
```

---

## 🔥 Usage  

### 🛠 Loading an APNG in Qt  
```cpp
#include <QImage>
#include <QMovie>
#include <QLabel>

// Load APNG as a QMovie
QMovie *movie = new QMovie("animated_image.apng");
QLabel *label = new QLabel;
label->setMovie(movie);
movie->start();
label->show();
```

---

## 🎯 Roadmap  

- [ ] Add **frame delay customization**  
- [ ] Improve **performance optimizations**  
- [ ] Add **APNG encoding support**  

---

## 🤝 Contributing  

Want to improve this plugin? Contributions are welcome!  

1. **Fork** the repository  
2. **Clone** your fork  
3. Create a new **feature branch**  
4. Submit a **Pull Request** 🎉  

For more details, see [CONTRIBUTING.md](CONTRIBUTING.md).  

---

## 📜 License  

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.  

---

## ⭐ Support  

If you find this project useful, please **⭐ Star** the repository and share it!  

📧 **Contact:** marcin.nowak.0628@proton.me
