# Custom Download Folder Fix
*Release 1.4.2 – August 2021*

- Fixes an issue with custom download location from "forgetting" permissions to acceess that folder after the app is restarted. 
  - This issue stems from Apple's tighly controlled security sandbox, where choosing a save location outside of the Desktop, Downloads, or Documents directories would require the user to select the save location again to properly save files. 
  - With this update, the app now uses a secure "bookmark" method of remembering and accessing the folder between launches of the app.
