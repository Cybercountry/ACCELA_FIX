# Source Code Installer

This repository is a fix/alternative for the official **ACCELA** installer, originally hosted at [ciscosweater/enter-the-wired](https://github.com/ciscosweater/enter-the-wired).

## The Fix

In the most recent versions of the original repository (such as `20260512222534`), the program is distributed in **AppImage** format. However, some users experience compatibility issues and execution failures with this packaging format.

To resolve this, this repository:
1. Removes the problematic AppImage package.
2. Brings back the **Python source code** files (from the `src` folder, along with `run.sh` and `requirements.txt`) from the stable version `20260425230142`.

The original ACCELA installation script is smart enough to detect the distribution type automatically. By finding the source code instead of the AppImage, it will set up a Python virtual environment (`.venv`) and install the necessary dependencies to run the system perfectly on your machine.

---

## Credits

**All credits for the original project go to [ciscosweater](https://github.com/ciscosweater).** The only modification made here was making the files from the previous source-based version available to work around the AppImage issue, using the same installation logic that the original author developed.

---

## How to Use


Follow the steps below in your terminal to clone the repository and complete the installation using our `RUN_ME` helper script.

### 1. Clone the Repository
Open your terminal and clone this repository to your machine:
```bash
git clone https://github.com/Cybercountry/ACCELA_FIX.git
```

### 2. Enter the Folder
```bash 
cd ACCELA_FIX
```

### 3. Run the Installer
To start the process, just run the main script:
```bash
./RUN_ME
```

The script has already been configured with the correct execution permissions (chmod +x). If for some reason your system blocks direct execution, you can force the permission by running:
`chmod +x RUN_ME`

**System Requirements:**
- Python3.

Since this installation uses Python source code, make sure you have Python installed on your system before starting.
