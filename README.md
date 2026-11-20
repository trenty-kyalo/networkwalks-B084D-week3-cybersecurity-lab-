# NETWORKWALKS ACADEMY
## WEEK 3 – CYBERSECURITY PRACTICAL LAB REPORT

**Student Name:** Trenty Kyalo  
**Course/Unit:** B084D – Cybersecurity  
**Assignment:** Week 3 Practical Exercises  
**Submission Date:** 20 November 2026

---

## 1. Introduction

This report documents the practical cybersecurity exercises undertaken during Week 3. The activities focused on password recovery using John the Ripper (JTR), the Networkwalks password-cracking tool, and preparation of an AI-assisted password-cracking environment using HexStrike AI.

The exercises were conducted on a Kali Linux environment using the supplied practice PDF files.

## 2. Practical Module 1 – John the Ripper

### Objective
To extract password hashes from password-protected PDF documents and attempt password recovery using John the Ripper.

### Tools Used
- Kali Linux
- John the Ripper
- `pdf2john`
- RockYou wordlist (`rockyou.txt`)

### Procedure
1. Navigated to the directory containing the supplied PDF files.
2. Used `pdf2john` to extract password hashes from the protected PDFs.
3. Saved the extracted hashes into separate hash files.
4. Used John the Ripper with the PDF format and RockYou wordlist to perform password recovery.
5. Used `john --show` to display recovered passwords.
6. Opened the original PDF documents using the recovered passwords to verify the results.

### Results

| Target file | Recovered password | Verification |
|---|---|---|
| My Locked PDF1.pdf | `good-luck` | Successfully opened |
| My Locked PDF2.pdf | `password1` | Successfully opened |
| My Locked PDF3.pdf | `1qaz2wsx` | Successfully opened |

**Outcome:** Successful. All three PDF passwords were recovered and verified by opening the original documents.

## 3. Practical Module 2 – Networkwalks Password Cracker

### Objective
To use the Networkwalks password-cracking platform to recover the password of a supplied protected PDF.

### Procedure
1. Accessed the Networkwalks password-cracking tool.
2. Submitted the required PDF/hash information.
3. Used the platform's password-cracking functionality.
4. Obtained the recovered password.
5. Opened the original PDF using the recovered password to confirm successful recovery.

**Outcome:** Successful. The password was recovered using the Networkwalks tool, and the original PDF opened successfully.

## 4. Optional Practical 1 – AI-Assisted Password Cracking

### Objective
To prepare an AI-assisted password-cracking environment using Claude Desktop and HexStrike AI MCP, allowing an AI assistant to interact with security tools such as John the Ripper.

### Environment Preparation
The following work was completed:

- Cloned the HexStrike AI repository.
- Installed Python 3.12 in a dedicated environment.
- Created and activated a Python virtual environment.
- Installed the required Python dependencies.
- Verified package compatibility.
- Confirmed that the essential server imports worked.
- Configured the HexStrike server to bind to `127.0.0.1` rather than all network interfaces.
- Started the HexStrike server locally.

### Verification

The server health endpoint returned HTTP `200 OK`.

The health response confirmed:
- Server status: Healthy
- John the Ripper availability: True
- Essential tools: 8/8 available
- Total available tools: 61

### Outstanding Work
Claude Desktop installation and MCP client integration were not completed before report preparation. Consequently, an AI-assisted password-cracking run was not verified.

The original optional lab attachment, `hash3.networkwalks_flag1.pdf`, was also not found in the supplied working files. The previously tested `My Locked PDF1.pdf` was identified as a possible substitute for demonstrating the workflow, but no completed AI-assisted run is claimed.

## 5. Optional Practical 2 – Mediroza Hospital Patient Portal

This optional exercise was not completed during the available practical session. No claim of testing, exploitation, or access to patient information is made.

## 6. Challenges Encountered

1. **Python compatibility:** The available system Python version caused compatibility considerations during HexStrike installation. A dedicated Python 3.12 environment was therefore created.
2. **Dependency management:** Dependencies were installed and checked using `uv`.
3. **Server network configuration:** The server's binding address was adjusted to use localhost for safer local operation.
4. **Missing lab attachment:** The specified `hash3.networkwalks_flag1.pdf` file was not present in the working directory.

## 7. Conclusion

The required password-cracking exercises were successfully completed. John the Ripper recovered the passwords of three protected PDF documents, and each result was verified by opening its corresponding original file. The Networkwalks password-cracking exercise was also completed successfully.

The HexStrike AI environment was installed and its server health verified, although Claude Desktop integration remained outstanding. The second optional exercise was not completed.

The practical work provided hands-on experience with password hash extraction, dictionary-based password recovery, tool verification, Python environment management, and local security-tool server configuration.

---

**End of Report**
