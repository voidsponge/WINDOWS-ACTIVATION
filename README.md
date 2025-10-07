# Windows Activation Script

## ⚠️ Important Warning

This script uses a third-party tool for Windows activation. Please note that:

- Using this script is **at your own risk**
- Make sure to comply with Microsoft's license terms
- It is recommended to purchase a legitimate Windows license
- This README is provided for informational purposes only

## 📋 Description

This PowerShell script allows you to run a Windows activation tool via a simplified command.

## 🚀 Usage

### Prerequisites

- Windows 10 or Windows 11
- PowerShell 5.1 or higher
- Active Internet connection
- Administrator rights

### Installation

1. Open PowerShell **as administrator**:
   - Right-click on the Start menu
   - Select "Windows PowerShell (Admin)" or "Terminal (Admin)"

2. Run the following command:

```powershell
irm https://get.activated.win/ | iex
```

### Command Explanation

- `irm`: Alias for `Invoke-RestMethod` - downloads content from the URL
- `|`: Pipeline - passes the result to the next command
- `iex`: Alias for `Invoke-Expression` - executes the downloaded script

## 🔒 Security

### Recommendations

- Always verify the source of scripts before executing them
- Use up-to-date antivirus software
- Create a system restore point before running the script
- Read the source project documentation to understand the actions performed

### Creating a Restore Point

Before running the script, create a restore point:

```powershell
Checkpoint-Computer -Description "Before Windows activation" -RestorePointType "MODIFY_SETTINGS"
```

## ❓ FAQ

### The script doesn't work

- Verify that you're running PowerShell as administrator
- Make sure your Internet connection is active
- Check that script execution is allowed: `Set-ExecutionPolicy RemoteSigned -Scope CurrentUser`

### Is this legal?

Using unofficial activation tools may violate Microsoft's terms of service. It is strongly recommended to purchase a legitimate Windows license.

### Legitimate Alternatives

- Purchase a Windows license from the Microsoft Store
- Use Windows with a Microsoft account (digital activation)
- Take advantage of student or business offers if you're eligible

## 📝 License

This README is provided for informational purposes only. Use of the activation script is subject to the terms of the source project.

## 🔗 Useful Links

- [Official Microsoft Website](https://www.microsoft.com/en-us/windows)
- [Buy a Windows License](https://www.microsoft.com/en-us/store/b/windows)
- [Microsoft Support](https://support.microsoft.com/)

## ⚖️ Disclaimer

This project is not affiliated with Microsoft Corporation. Windows is a registered trademark of Microsoft. The author of this README cannot be held responsible for the use of this script.

---

**Note**: Always prioritize purchasing a legitimate Windows license to support developers and benefit from official support.
