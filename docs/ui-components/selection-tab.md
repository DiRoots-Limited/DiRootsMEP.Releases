---
layout: default
title: Insulation Tools
parent: User Guide
nav_order: 1
---

# Insulation Tools
{: .no_toc }
The insulation tools helps users to easily manage, review and apply insulation for pipes and ducts.
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Add Insulation

This feature allows users to automatically apply insulation to pipes and ducts based on predefined rules such as size, workset, and comments. 


### Interface Overview

The tool contains two main tabs — Pipes and Ducts, allowing users specify which elements to apply insulation to.

### Selection Scope

Filtering options available:

Before creating rules, choose the scope of selection
1. Whole Model – Applies the rule to all relevant elements in the model.
2. Active View – Applies the rule to elements visible in the current view.
3. Current Selection – Applies the rule only to currently selected elements.


### Add Rules

Click Add Rule to define custom rules for insulation application.

![DiRootsMEP Add Insulation Tool - Add Rule](../../assets\images\GIFs\InsulationTools\AddInsulation\DMEP_Insulation-Tools-Add-Insulation-Add-Rule.gif)  
<sub>Note: the version on the image may not reflect the [latest version of DiRootsMEP](https://diroots.com/revit-plugins/dirootsmep/).</sub>

### Preferences

Set preferences those needed to be included in the rule like Size range, System type, Worksets and Custom parameters, from the preferences list. In Custom parameters you can select a predefined or custom parameters from the dropdown menu.


![DiRootsMEP Add Insulation Tool - Add Rules - Preferences](../../assets\images\GIFs\InsulationTools\AddInsulation\DMEP_Insulation-Tools-Add-Insulation-Add-Rule-Preferences.gif)  
<sub>Note: the version on the image may not reflect the [latest version of DiRootsMEP](https://diroots.com/revit-plugins/dirootsmep/).</sub>

### Auto Update

Enable Auto Update if you want insulation to be automatically applied to newly created pipes or ducts that match the defined rules.

![DiRootsMEP Add Insulation Tool - Auto Update](../../assets\images\GIFs\InsulationTools\AddInsulation\DMEP_Insulation-Tools-Add-Insulation-Auto-update.gif)  
<sub>Note: the version on the image may not reflect the [latest version of DiRootsMEP](https://diroots.com/revit-plugins/dirootsmep/).</sub>

### Save and Apply

Once all rules are configured, click Save and Apply to implement them across the Sope you have selected(Whole Model, Active View and Current selection).

![DiRootsMEP Add Insulation Tool - Save and Apply](../../assets\images\GIFs\InsulationTools\AddInsulation\DMEP_Insulation-Tools-Add-Insulation-Save-and-Apply.gif)  
<sub>Note: the version on the image may not reflect the [latest version of DiRootsMEP](https://diroots.com/revit-plugins/dirootsmep/).</sub>

### Expor/Import

Export: Save your insulation rules as a .json file for future reuse or sharing.

![DiRootsMEP Add Insulation Tool - Export](../../assets\images\GIFs\InsulationTools\AddInsulation\DMEP_Insulation-Tools-Add-Insulation-Export.gif)  
<sub>Note: the version on the image may not reflect the [latest version of DiRootsMEP](https://diroots.com/revit-plugins/dirootsmep/).</sub>

Import: Load an existing .json file to quickly apply previously defined rules.

![DiRootsMEP Add Insulation Tool - Import](../../assets\images\GIFs\InsulationTools\AddInsulation\DMEP_Insulation-Tools-Add-Insulation-Import.gif)  
<sub>Note: the version on the image may not reflect the [latest version of DiRootsMEP](https://diroots.com/revit-plugins/dirootsmep/).</sub>
  
---

## Hide Insulation

Use this feature to temporarily hide insulation for selected pipes or ducts in the model. Simply select the elements and click Hide Insulation — the insulation will be visually hidden without removing it.

![DiRootsMEP Hide Insulation](../../assets\images\GIFs\InsulationTools\HideInsulation\DMEP_Insulation-Tools-Hide-Insulation.gif)  
<sub>Note: the version on the image may not reflect the [latest version of DiRootsMEP](https://diroots.com/revit-plugins/dirootsmep/).</sub>
