# Email & Password Profiler (OSINT Tool)

A Python-based tool to generate and verify email IDs based on user-provided personal information and integrate with the Zeruh API for email validation. This tool also includes a password generator to create potential password combinations.

![image](https://github.com/user-attachments/assets/b0e5bb54-931e-4f31-a0bc-417d07cebb46)



## Overview

The Email & Password Profiler helps users generate email address variations using first name, last name, and date of birth, verify them against the Zeruh API, and create password suggestions based on personal details. It features a graphical user interface built with PySimpleGUI, making it user-friendly for both technical and non-technical users.

![image](https://github.com/user-attachments/assets/aacc400c-8e9b-4aaa-8b11-c5f5b2aa23ae)

![image](https://github.com/user-attachments/assets/54102ebb-5f35-4b77-97c3-7d5fc8d79f4f)


## Features

- Generate email IDs from personal details (first name, last name, DOB) with customizable domains.
- Verify email deliverability using the Zeruh API.
- Interactive tree view to select and manage generated emails.
- Password generator with options for word variations, numbers, special characters, and Leet Speak.
- Save and load profiles to persist user data.
- Filter emails by domain and export results to CSV.

## Prerequisites

- Python 3.6 or higher
- Required Python packages:
  - `PySimpleGUI`
  - `pillow` (PIL)
  - `requests`
  - `webbrowser` (included in Python standard library)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/email_pswd_osint_tool.git
   cd email_pswd_osint_tool
2. python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
3. pip install PySimpleGUI pillow requests
4. Obtain a Zeruh API key:
Register at https://my.zeruh.com/account/register.
Set the API key in the tool via the 'Tools' > 'Set Zeruh API Key...' menu.

# Usage

Run the tool:
```bash
python email_pswd_osint_tool.py
```

1. Enter user information (First Name, Last Name, Date of Birth in YYYY-MM-DD format).
2. Add custom domains (one per line) or use default domains (e.g., gmail.com, yahoo.com).
3. Click "Generate Email IDs" to create email variations.
4. Select emails in the tree view and click "Verify Selected (API)" to check deliverability (requires API key).
5. Use the 'Tools' menu to access the password generator or register for a Zeruh API account.
6. Save profiles or export verified emails to a CSV file via the 'File' menu.

### The more information you provide, the greater number of passwords will be generated. 

# Example

- **Input:** First Name = "John", Last Name = "Doe", DOB = "1990-01-01"
- **Generated Emails:** johndoe@gmail.com, jdoe@yahoo.com, etc.
- **Verification:** Marks johndoe@gmail.com as "Valid" if deliverable (per Zeruh API).
- **Passwords:** Generates JohnDoe, jdoe1990, J0hnD0e!, etc., based on generator settings.

# Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Make your changes and commit: `git commit -m "Description of changes"`.
4. Push to the branch: `git push origin feature-name`.
5. Submit a pull request.

# License

This project is licensed under the MIT License - see the LICENSE file for details.

# Disclaimer

<b>This tool is intended for legitimate use only, such as personal research or security testing with proper authorization. Misuse for unauthorized access or malicious purposes is prohibited and may violate laws.</b>
