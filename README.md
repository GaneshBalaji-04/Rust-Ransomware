# 🚀 Rust-Based Ransomware for Windows  
This project is a **Rust-powered ransomware** designed to encrypt files and folders. It leverages **Windows API calls** to enhance its robustness and efficiency.  

## 🔥 Why Rust?  
Rust compiles using **LLVM**, introducing additional complexity and optimization, making it significantly harder to **reverse engineer** and understand the original code.  

> ⚠️ **Warning:** Do **NOT** run this on your personal system—it will encrypt all your files! Always test in a **virtual machine**.  

## ⚖️ Disclaimer  
- This project is intended **strictly for educational purposes**. The developers hold **no responsibility** for any misuse.  
- Running this on your main system **will encrypt personal files**. Only test in a **virtual environment**.  
- The **Cargo compiler must be installed** to build the executable. The recommended way to compile is:  

  ```
  cargo build --release
  ```

# 🚀 Standalone Executable Advantage
Rust compiles to **native machine code**, meaning the final `.exe` file can run on Windows **without requiring the Rust compiler**.

- The `--release` flag ensures an optimized and standalone executable.

- The compiled `.exe` will be located in:
  ```
  target/release/executable.exe
  ```

- Since Rust **statically links** most of the dependencies, the final executable is often **self-contained** and **does not need Rust installed on the target system.**

# 📦 Required Libraries
The following libraries are used in this project:
- `Iced`
- `Winapi`
- `Windows`
- `Reqwest`
- `Tokio`
- `Rand`
- `Warp`
- `Base64`
- `RSA`

# 🚀 How to Try It?

1. **Clone the repository** or **download the ZIP file** inside a virtual machine.
    ```
    git clone https://github.com/GaneshBalaji-04/Rust-Ransomware.git
    cd Rust-Ransomware
    ```

2. If using a ZIP file, extract it into your preferred folder.
    - For more fun, **run the server on the host OS** while the **client runs inside the virtual machine.**

3. **Compile the executable:**
    ```
    cargo build --release
    ```

4. Run the `.exe` file.

💡 Feel free to fork this repository and modify it as needed! 🎯

## 📝 License  

This project is licensed under the **MIT License**. See the LICENSE file for more details.  
Copyright (c) 2024 Ganesh Balaji V and Dharineesh J.