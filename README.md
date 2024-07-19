# CrowdStrike-Fix

## Description

CrowdStrike-rollback.ps1 is a PowerShell script designed to automate the process of removing a specific file related to CrowdStrike that may be causing issues on your Windows system. This script should be run in Safe Mode or in the Windows Recovery Environment.

## Problem with CrowdStrike

CrowdStrike is a security solution that protects endpoints against threats. However, in some situations, certain CrowdStrike files can become corrupted or cause problems that prevent the system from functioning properly. In this specific case, a file named `C-00000291*.sys` in the `C:\Windows\System32\drivers\CrowdStrike` directory needs to be removed to resolve the issue.

## Usage Instructions

### Step 1: Preparation

- Ensure that you have administrator permissions on the system where the script will be executed.
- Save the script to a file named `CrowdStrike-rollback.ps1`.

### Step 2: Boot into Safe Mode

1. Restart the system and boot into Safe Mode or the Windows Recovery Environment.
2. To enter Safe Mode, hold down the **Shift** key while clicking "Restart" and then select:
   - "Troubleshoot"
   - "Advanced options"
   - "Startup Settings"
   - "Restart"
   - Then, select the option for Safe Mode.
3. To enter the Windows Recovery Environment, follow a similar process and select:
   - "Troubleshoot"
   - "Advanced options"
   - "Command Prompt".

### Step 3: Run the Script

1. Open PowerShell with administrator privileges.
2. Navigate to the directory where the script was saved.
3. Run the script with the following command:

   ```powershell
   .\CrowdStrike-fix.ps1
   ```

I hope this helps to at least automate the issue to some extent.
