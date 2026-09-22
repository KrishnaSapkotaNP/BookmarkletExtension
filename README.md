# ERP Attendance Extension

A browser-based tool that extracts attendance data directly from ERP webpages and converts it into a clean, structured format.

The project is designed to work across different college and university ERP systems instead of being tied to a single institution.

---

## Features

* Automatically detects attendance tables
* Extracts course code and subject name
* Extracts present and absent counts
* Calculates attendance percentage automatically
* Runs directly in the browser
* No need to manually copy attendance data
* Works as a browser bookmarklet

---

## How It Works

The tool runs as a **bookmarklet**, allowing it to execute directly on an ERP webpage without installing a browser extension.

It:

1. Scans the webpage for tables.
2. Identifies tables that contain attendance information.
3. Reads the table headers and rows.
4. Extracts relevant attendance fields.
5. Normalizes the data into a common structure.
6. Calculates the attendance percentage.

### Attendance Calculation

```text
Attendance % = Present Count / Total Count × 100
```

---

## How to Use

No installation is required.

### 1. Create a Bookmark

Create a new bookmark in your browser and give it a name such as:

```text
ERP Attendance
```
or just drag to the bookmark tab by clicking CTRL+SHIFT+B
### 2. Add the Bookmarklet Code

Copy the bookmarklet code provided in this repository and paste it into the **URL / Address** field of the bookmark.

The bookmark should look like:

```text
Name: ERP Attendance
URL: javascript:...
```

### 3. Open Your ERP Attendance Page

Log in to your college or university ERP and navigate to the page containing your attendance table.

### 4. Run the Bookmarklet

Click the **ERP Attendance** bookmark.

The bookmarklet will scan the current webpage, extract the attendance data, and display the structured results.

---

## Browser Support

Because this is a bookmarklet, it does not require a browser extension or installation from a browser web store.

It can be used in modern browsers that support JavaScript bookmarklets, including:

* Google Chrome
* Microsoft Edge
* Brave
* Mozilla Firefox
* Opera
* Other Chromium-based browsers

---

## Privacy

The tool processes attendance data directly from the webpage in the browser.

No attendance data needs to be manually uploaded to a server for the extraction process.

---

## Project Goal

The goal of this project is to create a **generic attendance extraction tool** that can work with different ERP systems by identifying attendance information based on table structure and column patterns rather than relying on a single college's ERP layout.
