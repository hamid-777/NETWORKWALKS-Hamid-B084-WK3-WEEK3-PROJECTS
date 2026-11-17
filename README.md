# Week 03 – Password Cracking Lab

## 1. Introduction

This lab focuses on understanding password cracking techniques and recovering passwords from password-protected PDF files.

The objective was to extract the PDF password hash and use password-cracking tools to recover the original password.

Two methods were performed:

- **Method 1:** John the Ripper with Johnny GUI.
- **Method 2:** Networkwalks Hash Calculator and Password Cracker.

---

## 2. Lab Environment

| Component | Details |
|---|---|
| **Operating System** | Windows |
| **Password Cracking Tool** | John the Ripper |
| **Graphical Interface** | Johnny GUI |
| **Hash Extraction Tool** | Networkwalks Hash Calculator |
| **Online Cracking Tool** | Networkwalks Password Cracker |
| **Target File** | Password-protected PDF |

---

# Part 1 – John the Ripper & Johnny GUI

## Step 1 – Download John the Ripper

1. Open the official Openwall website: [https://www.openwall.com/john/](https://www.openwall.com/john/)
2. Download John the Ripper for Windows.
3. Extract the downloaded archive.
4. Locate the `run` folder.
5. Verify that `john.exe` is available inside the folder.

## Step 2 – Download and Install Johnny GUI

1. Visit the official Johnny website: [https://openwall.info/wiki/john/johnny](https://openwall.info/wiki/john/johnny)
2. Download Johnny GUI.
3. Run the installation file.
4. Complete the installation.
5. Open Johnny GUI.

## Step 3 – Configure Johnny GUI

1. Open Johnny.
2. Navigate to **Settings**.
3. Browse for the John the Ripper executable.
4. Select `john.exe` from the extracted `run` folder.
5. Save the configuration.

## Step 4 – Download the Encrypted PDF

1. Download the password-protected PDF file to your Windows computer.
2. Keep the file in an accessible location.

## Step 5 – Extract the PDF Hash

1. Open the Online Hash Extractor: [https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php)
2. Browse and select the encrypted PDF file.
3. Click **Upload**.
4. Copy the extracted PDF hash.

**Note:** The extracted hash should start with `$pdf$`. Remove any extra characters, such as `b'`, if they appear in the copied output.

## Step 6 – Save the Hash

1. Open **Notepad**.
2. Paste the complete PDF hash.
3. Select **File → Save As**.
4. Enter the filename `hash1.txt`.
5. Save the file as a text document.

## Step 7 – Load the Hash into Johnny

1. Open Johnny GUI.
2. Click **Open Password File**.
3. Browse to the `hash1.txt` file.
4. Select the file and click **Open**.
5. Verify that the hash has been loaded.

## Step 8 – Start the Password Cracking Attack

1. Click **Start New Attack**.
2. Allow John the Ripper to process the hash.
3. Wait for the password recovery process to finish.
4. Review the recovered password in Johnny.

**Note:** The time required depends on the password complexity and computer performance.

### Screenshot

<img width="1280" height="747" alt="jhonny" src="https://github.com/user-attachments/assets/a8965e89-c06c-473b-bd39-9b2330905b33" />

## Step 9 – Verify the Recovered Password

1. Open the encrypted PDF.
2. Enter the recovered password.
3. Verify that the PDF opens successfully.

### Screenshots

<img width="1917" height="1185" alt="pdf1" src="https://github.com/user-attachments/assets/4c12620f-330b-4381-a32b-18a9a956afcd" />

<img width="1917" height="1167" alt="pdf2" src="https://github.com/user-attachments/assets/5b029aea-d86e-4680-82e8-9518ddd8aad4" />

<img width="1917" height="1172" alt="pdf3" src="https://github.com/user-attachments/assets/23ea070b-f2b3-4ba2-ba81-19a31fb2dd83" />

---

# Part 2 – Networkwalks Online Tools

## Step 1 – Download the Lab PDF

1. Visit the Networkwalks lab page: [Networkwalks Password Cracking Lab](https://networkwalks.com/project-task-lab-password-cracking-with-networkwalks-tools/)
2. Download the encrypted PDF file named `My Locked PDF1.pdf`.
3. Save it to your Windows computer.

## Step 2 – Open the Hash Calculator

1. Open a web browser.
2. Visit the [Networkwalks Hash Calculator](https://networkwalks.com/hash-calculator/).
3. Locate the PDF hash extraction option.

## Step 3 – Extract the PDF Hash

1. Upload `My Locked PDF1.pdf`.
2. Allow the tool to process the file.
3. Copy the generated PDF hash.
4. Ensure the complete hash is copied, starting with `$pdf$`.

## Step 4 – Open the Password Cracker

1. Open a new browser tab.
2. Visit the [Networkwalks Password Cracker](https://networkwalks.com/password-cracker/).
3. Locate the hash input field.

## Step 5 – Perform the Password Cracking Attack

1. Paste the extracted PDF hash into the Password Cracker.
2. Start the password-cracking process.
3. Wait for the tool to complete the attack.
4. Review the recovered password displayed on the screen.

**Note:** The time required depends on password complexity and the resources available to the tool.

### Screenshot

<img width="1917" height="1117" alt="NW password cracker" src="https://github.com/user-attachments/assets/054ac2bc-a688-4aa3-b7f3-7431b447a2ec" />


## Step 6 – Verify the Password

1. Locate the downloaded `My Locked PDF1.pdf` file.
2. Open the PDF.
3. Enter the recovered password.
4. Confirm that the protected document opens successfully.

---

## 3. Tools and Technologies Used

| Tool | Purpose |
|---|---|
| **John the Ripper** | Password recovery |
| **Johnny GUI** | Graphical interface for John the Ripper |
| **Networkwalks Hash Calculator** | Extracting PDF password hashes |
| **Networkwalks Password Cracker** | Recovering passwords from hashes |
| **Notepad** | Saving extracted hashes |
| **Windows** | Lab operating system |

---

## 4. Skills and Concepts Learned

- **Password Hashing:** Understanding how passwords are represented by hashes.
- **Hash Extraction:** Extracting password hashes from protected PDF files.
- **Dictionary-Based Attacks:** Understanding how password-cracking tools test possible passwords.
- **John the Ripper:** Performing password recovery using a command-line-based cracking engine.
- **Johnny GUI:** Configuring and using a graphical interface for John the Ripper.
- **Online Password Cracking:** Using browser-based tools for hash extraction and password recovery.
- **Password Security:** Understanding the importance of password complexity and strong password policies.

---

## 5. Conclusion

Successfully completed **Week 3** of the Networkwalks cybersecurity practical training.

Performed PDF password recovery using two different approaches: **John the Ripper with Johnny GUI** and **Networkwalks online tools**.

The lab provided practical experience in extracting password hashes, conducting password-cracking attacks, and understanding the security risks associated with weak passwords.

**Lab Status:** Completed :white_check_mark:

---

## 6. References

1. [John the Ripper – Official Website](https://www.openwall.com/john/)
2. [Johnny GUI – Openwall](https://openwall.info/wiki/john/johnny)
3. [Online PDF Hash Extractor](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php)
4. [Networkwalks Hash Calculator](https://networkwalks.com/hash-calculator/)
5. [Networkwalks Password Cracker](https://networkwalks.com/password-cracker/)
6. [Networkwalks Password Cracking Lab Instructions](https://networkwalks.com/project-task-lab-password-cracking-with-networkwalks-tools/)

---

## 7. Disclaimer

All activities were performed for educational purposes using authorized lab files.

Password recovery should only be conducted on files and systems for which permission has been granted.

---

**Training:** Networkwalks  
**Week:** 03  
**Topic:** Password Cracking  
**Status:** Completed
