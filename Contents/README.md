# 📄 BumbleBeeZ – Dynamic Content Update

This document explains how to manage the `credits.json` and `updates.json` files used in the BumbleBeeZ application.  
These files allow content to be updated dynamically without requiring frequent app redeployment.

---

## 🎖 Credits Configuration

# 🧾 Format Structure

Each entry should follow this format:

```json
{
  "Name of the member": "Role of the member"
}
```

### ✅ Example

```json
{
  "Rishi Aravind": "Developer & Consultant",
  "Prakash Antony": "Developer & Consultant",
  "Mohanam": "Survey Helper",
  "Praveen": "Site Manager"
}
```

---

## 🚀 Updates Configuration

### 🧾 Format Structure

Each entry should follow this format:

```json
{
  "<dd/mm/YYYY>: <Title of the update>": "Description of the update"
}
```

### ✅ Example

```json
{
  "28/06/2025: Initial Public Release": "BumbleBeeZ launched with core features like account creation and role-based access.",
  "30/06/2025: UI Improvements": "Improved layout and added icons to enhance user experience.",
  "02/07/2025: Location Services Added": "Enabled GPS access for real-time field tracking by survey helpers."
}
```

---

## 💡 Tips

- Keep titles and names short but meaningful.
- Write clear and concise descriptions or roles.
- Make sure the date format is **dd/mm/yyyy** in updates.
- Do **not** add commas after the last item in any JSON object.
- If you want to add internal notes, use a special field like `_comment`:

```json
{
  "_comment": "This file contains visible app update logs. Avoid using // or # for comments.",
  "10/07/2025: Accessibility Update": "Improved keyboard navigation and screen reader support."
}
```

> ⚠️ `_comment` fields will be ignored by the app but can help document the file for contributors.

---

## 📌 Usage in App

- These files are fetched dynamically and rendered in the **Credits** and **Updates** pages of the app.
- Any content change in these JSON files is reflected **instantly** for all users without needing an app update.

---

## 📬 How to Contribute

To add a new credit or update entry:
1. Open the relevant JSON file inside `/Contents/`.
2. Follow the format guidelines above.
3. Commit your changes to the repository.

---
