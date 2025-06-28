# 📄 BumbleBeeZ – Dynamic Content Update

This file is dynamically updated without requiring app patch updates or redeployment.

---

## 🎖 Credits Configuration

### 🧾 Format Structure

Each entry must follow this format:

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

**Note:** New updates should always be added at the beginning of the JSON object (stack format), so the latest updates appear first on the screen.

### 🧾 Format Structure

Each update must follow this format:

```json
{
  "<dd/mm/YYYY>: <Title of the update>": "Description of the update"
}
```

### ✅ Example

```json
{
  "02/07/2025: Location Services Added": "Enabled GPS access for real-time field tracking by survey helpers.",
  "30/06/2025: UI Improvements": "Improved layout and added icons to enhance user experience.",
  "28/06/2025: Initial Public Release": "BumbleBeeZ launched with core features like account creation and role-based access."
}
```

---
