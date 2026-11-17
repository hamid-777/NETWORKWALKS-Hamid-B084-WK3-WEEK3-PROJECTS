Week 03 – Password Cracking Lab

1. Introduction

This lab focuses on understanding password cracking techniques and recovering passwords from password-protected PDF files.

The objective was to extract the PDF password hash and use password-cracking tools to recover the original password.

Two methods were performed:

John the Ripper with Johnny GUI.

Networkwalks Hash Calculator and Password Cracker.

2. Lab Environment

Component

Details

Operating System

Windows

Password Cracking Tool

John the Ripper

Graphical Interface

Johnny GUI

Hash Extraction

Networkwalks Hash Calculator

Online Cracking Tool

Networkwalks Password Cracker

Target File

Password-protected PDF

Part 1 – John the Ripper & Johnny GUI

Step 1 – Download John the Ripper

Open the official Openwall website:
https://www.openwall.com/john/

Download John the Ripper for Windows.

Extract the downloaded archive.

Locate the run folder.

Verify that john.exe is available inside the folder.

Step 2 – Download and Install Johnny GUI

Visit the official Johnny website:
https://openwall.info/wiki/john/johnny

Download Johnny GUI.

Run the installation file.

Complete the installation.

Open Johnny GUI.

Step 3 – Configure Johnny GUI

Open Johnny.

Navigate to Settings.

Browse for the John the Ripper executable.

Select john.exe from the extracted run folder.

Save the configuration.

Step 4 – Download the Encrypted PDF

Download the password-protected PDF file to the Windows computer.

Keep the file in an accessible location.

Step 5 – Extract the PDF Hash

Open the Online Hash Extractor:
https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php

Browse and select the encrypted PDF file.

Click Upload.

Copy the extracted PDF hash.

Note: The extracted hash should start with $pdf$. Remove any extra characters, such as b', if they appear in the copied output.

Step 6 – Save the Hash

Open Notepad.

Paste the complete PDF hash.

Select File → Save As.

Enter the filename hash1.txt.

Save the file as a text document.

Step 7 – Load the Hash into Johnny

Open Johnny GUI.

Click Open Password File.

Browse to the hash1.txt file.

Select the file and click Open.

Verify that the hash has been loaded.

Step 8 – Start the Password Cracking Attack

Click Start New Attack.

Allow John the Ripper to process the hash.

Wait for the password recovery process to finish.

Review the recovered password in Johnny.

The time required depends on the password complexity and computer performance.

Step 9 – Verify the Recovered Password

Open the encrypted PDF.

Enter the recovered password.

Verify that the PDF opens successfully.

Part 2 – Networkwalks Online Tools

Step 1 – Download the Lab PDF

Visit the Networkwalks lab page:
https://networkwalks.com/project-task-lab-password-cracking-with-networkwalks-tools/

Download the encrypted PDF file named My Locked PDF1.pdf.

Save it to the Windows computer.

Step 2 – Open the Hash Calculator

Open a web browser.

Visit:
https://networkwalks.com/hash-calculator/

Locate the PDF hash extraction option.

Step 3 – Extract the PDF Hash

Upload My Locked PDF1.pdf.

Allow the tool to process the file.

Copy the generated PDF hash.

Ensure the complete hash is copied, starting with $pdf$.

Step 4 – Open the Password Cracker

Open a new browser tab.

Visit:
https://networkwalks.com/password-cracker/

Locate the hash input field.

Step 5 – Perform the Password Cracking Attack

Paste the extracted PDF hash into the Password Cracker.

Start the password-cracking process.

Wait for the tool to complete the attack.

Review the recovered password displayed on the screen.

Step 6 – Verify the Password

Locate the downloaded My Locked PDF1.pdf file.

Open the PDF.

Enter the recovered password.

Confirm that the protected document opens successfully.

3. Tools and Technologies Used

Tool

Purpose

John the Ripper

Password recovery

Johnny GUI

Graphical interface for John the Ripper

Networkwalks Hash Calculator

Extracting PDF password hashes

Networkwalks Password Cracker

Recovering passwords from hashes

Notepad

Saving extracted hashes

Windows

Lab operating system

4. Skills and Concepts Learned

Password hashing and hash extraction.

PDF password protection.

Dictionary-based password attacks.

Password recovery using John the Ripper.

Configuring and using Johnny GUI.

Using online password-cracking tools.

Understanding password complexity and security.

5. Conclusion

Successfully completed Week 3 of the Networkwalks cybersecurity practical training.

Performed PDF password recovery using two different approaches: John the Ripper with Johnny GUI and Networkwalks online tools.

The lab provided practical experience in extracting password hashes, conducting password-cracking attacks, and understanding the security risks associated with weak passwords.

Lab Status: Completed

Disclaimer: All activities were performed for educational purposes on authorized lab files. Password recovery should only be conducted on files and systems for which permission has been granted.
