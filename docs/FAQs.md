---
layout: default
title: FAQs
nav_order: 99
---

# Frequently Asked Questions about DiRootsMEP

This section aims to answer the our users' frequently asked questions.


## Why does DiRootsMEP show "No Internet Connection"?

If you see the error **"Please check your internet connection"** while using DiRootsMEP, here's what it means and how to fix it:

### Why this happens
- **License Verification**: DiRootsMEP needs an active internet connection to validate premium subscriptions.   

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