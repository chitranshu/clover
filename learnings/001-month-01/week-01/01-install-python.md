# Install Python and Set Up Environment

## Step 1: Install Python
- Go to the official Python website: https://www.python.org/downloads/
- Download the latest stable version of Python (e.g., Python 3.11 or later).
- Run the installer and follow the prompts.
- Make sure to check the box that says "Add Python to PATH" during installation.

## Step 2: Verify Installation
- Open a terminal or command prompt.
- Type `python --version` and press Enter. You should see the installed Python version.
- Type `pip --version` to verify that pip (Python package installer) is also installed

## Step 3: Set Up a Virtual Environment (Optional but Recommended)
- Navigate to your project directory in the terminal.
- Run the following command to create a virtual environment:
```bash
python -m venv .venv
```
- Activate the virtual environment:
- On Windows:
```bash
.venv\Scripts\activate
```
- On macOS/Linux:
```bash
source .venv/bin/activate
```
- You should see the virtual environment name in your terminal prompt, indicating that it is active.
