# Nmap_shell_scripting

**Nmap Script - Network Scanning Tool**

**Description**

This script provides a user-friendly interface to perform basic network scans using the powerful `nmap` tool. It allows you to choose between normal scans, TCP scans, and UDP scans for a specified hostname.

**Requirements**

- Linux or macOS system
- `nmap` tool installed (usually available through the package manager)
- Root or sudo privileges to execute `nmap`

**Installation**

1. **Save the Script:**
   Create a file named `nmap_scanner.sh` (or any preferred name) and paste the code provided.

2. **Make the Script Executable:**
   Open a terminal and navigate to the directory where you saved the script. Use the following command:

   ```bash
   chmod +x nmap_scanner.sh
   ```

   This grants the script permission to be executed.

**Usage**

1. **Run the Script:**
   Open a terminal and navigate to the directory containing the script. Then, execute it using the following command:

   ```bash
   ./nmap_scanner.sh
   ```

2. **Follow the Prompts:**
   The script will first ask you to enter the hostname of the system you want to scan.
   Next, you'll be prompted to enter your system password for using `sudo` (required to run `nmap` with elevated privileges). The password will not be echoed on the screen for security reasons.

3. **Select Scan Type:**
   The script will display a menu with three options:

   - 1. Normal Scan
   - 2. TCP Scan
   - 3. UDP Scan

   Enter the corresponding number for the type of scan you want to perform.

4. **Scan Results:**
   The script will execute the `nmap` command with the chosen options and display the scan results directly in the terminal.

**Examples**

1. Scanning a host named `server1` with a normal scan:

   ```
   Enter the hostname: server1
   Enter system password: (type your password here, it won't be shown)

   1. Normal Scan
   2. TCP Scan
   3. UDP Scan

   Choose option which you want to prefer: 1

   ----------Normal Scan-----------
   # Output of the nmap scan for server1
   ```

2. Scanning a host named `router` with a UDP scan:

   ```
   Enter the hostname: router
   Enter system password: (type your password here, it won't be shown)

   1. Normal Scan
   2. TCP Scan
   3. UDP Scan

   Choose option which you want to prefer: 3

   ----------UDP Scan-----------
   # Output of the nmap UDP scan for router
   ```

**Disclaimer**

- Performing network scans without permission is illegal. Use this script responsibly and ethically.
- Network scans might trigger security measures on the target system. Use caution.

**Additional Notes**

- You can modify the script to include more advanced `nmap` options and scan types. Refer to the `nmap` documentation for details.
- Consider implementing error handling for invalid user input or scan failures.

I hope this comprehensive README file empowers you to effectively use this script for your network scanning needs!
