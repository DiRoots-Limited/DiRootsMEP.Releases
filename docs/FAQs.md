---
layout: default
title: FAQs
nav_order: 99
---

# Frequently Asked Questions about DiRootsMEP

This section aims to answer the our users' frequently asked questions.

## Does DiRootsMEP requires PDF24?

Yes. The correct version of PDF24 will be automatically installed alongside DiRootsMEP.

```
Uninstalling PDF24 will lead DiRootsMEP to stop working.
```

## Can I select another PDF printer?

No. DiRootsMEP works only with PDF24.

## What is the printer called diroots.dirootsmep that I got after installing DiRootsMEP?

diroots.dirootsmep printer is a custom instance of PDF24 that DiRootsMEP uses to set up its custom settings without affecting the main instance of PDF24.

## Why I can't see the PDFs being created in the output location?

If you don't see the PDF files appearing in the export path, it means that there are some issues with your settings. You can fix it, using one of the methods below.

**Method A**  

Open PDF24 -> Settings -> Printer Driver and confirm that your settings are as per the image below.

![DiRootsMEP Selecting Revit Sheets and Views](../assets\images\PS-Print-Settings.png)  

**Method B**  

1. uninstall DiRootsMEP and PDF24
2. download and install the [latest version of DiRootsMEP](https://diroots.com/revit-plugins/revit-to-pdf-dwg-dgn-dwf-nwc-ifc-and-images-with-dirootsmep/) from our website.
3. restart your computer and try again 

## Why I DiRootsMEP tells me that my printer is in an error state?

If DiRootsMEP is telling you that your printer is in error state, it means that the Windows printer services stopped working.  
Often, restart your computer is enough to fix the problem.

## Printer Permission Issue in DiRootsMEP (Failed to access print parameters)

### Problem
If you receive an error stating: `Unable to select Printer Printer Name` or `Failed to access print parameters`, this typically points to a printer driver or permissions issue that prevents DiRootsMEP from accessing complete printer information. Alternatively, it may indicate that no default printer is set on the system.

The Revit Print API works by first querying the available printers on the machine and then configuring the selected printer based on the format settings. Unfortunately, if any printer driver on the system is problematic, the Revit Print API may enter an error state. Even if the problematic printer is not actively in use, this error can still occur. Restarting Revit is often required to reset the error.

### Solution
**1. Identify the Default Printer**  
First, confirm that your system has a Default Printer. In Windows 10/11, there is an option called "Allow Windows to manage my default printer." If this option is enabled, your system automatically sets a default printer. If this is disabled, manually assign a default printer from the list of available devices.  

If the default printer is correctly set and the issue persists, proceed to identify the problematic printer driver by systematically disabling printers until the error clears.  

**2. Verify Printer Permissions**  
The user must have administrative permissions for the PDF24 Printer.  
To enable permissions:  
- Go to **Devices and Printers**.  
- Right-click on **PDF24 Printer** and select **Printer Properties**.  
- Navigate to the **Security** tab.  
- Ensure the following options are enabled for your user:  
   - **Manage this printer**  
   - **Manage documents**  

**3. Additional Considerations**  
If your printers are created via a login script or group policy, the problematic printer may reappear with each login. If this occurs, contact your **System Administrator** for further assistance in identifying and resolving the problematic printer driver.  

Several users have reported that the root cause of this issue was linked to a **network printer**. Identifying and disabling this printer often resolved the error.

By following these steps, you should be able to resolve printer-related issues when using **DiRoots DiRootsMEP** and **PDF24**.

## Why does DiRootsMEP show "No Internet Connection"?

If you see the error **"Please check your internet connection"** while using DiRootsMEP, here's what it means and how to fix it:

### Why this happens
- **License Verification**: DiRootsMEP needs an active internet connection to validate premium subscriptions.  
- **Export Tracking (Free Version)**: Free users have a monthly export limit, which must be verified online.  

If your internet is working but the error still appears, it's usually caused by your **firewall, proxy, or antivirus blocking DiRootsMEP/Revit**.

### How to fix it
1. **Check firewall/antivirus**: Make sure Revit/DiRootsMEP is not blocked.  
2. **Whitelist these domains**:  
   - `*.diroots.com`  
   - `*.dikeeper.com`  
   - `dikeeper-prod-euw-api-app-eefmhef2hhevbsgr.westeurope-01.azurewebsites.net`  
3. **Verify your connection**: Confirm you can access other online resources while using Revit.  
4. **Check DiRootsMEP logs** (if the issue persists):  

```
%localappdata%\DiRoots\DiRootsMEP\Log
```

Share the log files with our support team for further analysis.  

### Special case: Offline environments
DiRootsMEP does **not** work fully offline by default.  
If your organization requires an **offline license** (e.g., for secure IT environments), please contact DiRoots Support. Offline activation is available only under specific conditions.

---

✅ After restoring internet access or adjusting your firewall rules, DiRootsMEP should work as expected.