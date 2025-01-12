# Antivirus.exe

**Antivirus.exe** is a USB automation tool that creates a central folder to organize and store files from connected USB devices. It uniquely identifies each USB drive and stores its content in a structured manner, using either the USB name (if available) or a folder name based on the USB's size and connection date.

---

## Table of Contents

- [About the Project](#about-the-project)
- [How It Works](#how-it-works)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Usage](#usage)
- [Advantages](#advantages)
- [Disclaimer](#disclaimer)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## About the Project

**Antivirus.exe** is designed to automatically organize files from connected USB devices into a single directory called `UsbSystem` located in the `C:` drive. It creates a separate folder for each USB drive using the USB's name, or if no name is available, it generates a folder named based on the device's size and connection date.

---

## How It Works

1. **Centralized Storage:**
   - Creates a `UsbSystem` folder in the root of the `C:` drive.

2. **USB Detection:**
   - Automatically detects USB devices when they are connected.

3. **Folder Creation:**
   - For each USB device, it creates a folder inside `UsbSystem`:
     - If the USB drive has a name, it uses the name as the folder name.
     - If no name is available, it uses the size of the USB and the current date to generate a folder name in the format:  
       `Date[DD-MM-YYYY] Size[<size in bytes>]`

4. **File Management:**
   - Copies all files from the USB device to its corresponding folder.

5. **Stealth Operation:**
   - Operates silently in the background, ensuring minimal disruption.

---

## Features

- **Automated File Organization:** Detects and organizes USB files into a central directory.
- **Dynamic Folder Naming:** Uses USB name, or generates a name using size and connection date.
- **Stealth Mode:** Runs silently without user intervention.
- **Centralized Access:** All USB files are stored in one location for easy management.

---

## Getting Started

### Installation

1. **Download:**
   - Obtain the `Antivirus.exe` file from the source or repository.

2. **Setup:**
   - Place the executable in a location where it can monitor USB devices effectively.

### Usage

1. Run `Antivirus.exe`.
2. Connect any USB device to your system.
3. The program will automatically:
   - Create the `UsbSystem` folder in the `C:` drive (if it doesn’t already exist).
   - Create a unique subfolder for the USB device.
   - Copy all USB files into the subfolder.

4. Check the `C:\UsbSystem` directory to view the organized files.

---

## Advantages

- **Efficient File Management:** Automatically organizes USB files in a structured manner.
- **Portable:** Works with any USB device, regardless of the size or name.
- **Stealth Operation:** Runs quietly in the background without requiring user input.

---

## Example Folder Structure

For a USB drive connected on **01-01-2000** with a size of **123456789 bytes**, the folder structure will look like this:

```
C:\
└── UsbSystem\
    ├── MyUSBDrive\             # If USB has a name
    └── Date[01-01-2000] Size[1288610213]\  # If USB has no name
        ├── File1.txt
        ├── File2.jpg
        └── ...
```

---

## Disclaimer

This program is for **educational purposes only**. Unauthorized copying of files from USB drives may be unethical and violate privacy laws. Ensure you have permission before using this program on any USB device.

---

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m "Added feature XYZ"`).
4. Push to the branch (`git push origin feature-branch`).
5. Submit a Pull Request.

---

## License

This project is licensed under the **MIT License**. For details, see the `LICENSE` file.

---

## Contact

For feedback or support, please contact:

- GitHub: [spy-group](https://github.com/yourusername)
- Email: spy-group0@proton.me

---
