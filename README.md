# Instagram Follow Checker

A Python script to identify Instagram users you follow who don’t follow you back. It processes your Instagram follower and following data exported as JSON files and highlights non-mutual connections.

---

## Features

* **Load and parse Instagram follower and following data** from JSON files.
* **Extract usernames** from nested JSON structures reliably.
* **Compare follower and following lists** to identify users who don't follow you back.
* User-friendly output with clear notifications.

---

## Prerequisites

* Python 3.x installed
* Instagram data exported in JSON format (see below)

---

## Usage

### 1. Export Your Instagram Data

* Navigate to **Instagram Settings > Your Activity > Download Your Information**.
* Request your data in **JSON format**.
* Instagram will send you a download link via email.
* Extract the archive, locate the relevant `followers.json` and `following.json` files (or similarly named files).
* Ensure these JSON files contain the follower/following data with usernames in a consistent structure.

### 2. Prepare Files

* Place the JSON files in the same directory as the script.
* Rename them as needed (e.g., `followers.json` and `following.json`) to match the script's expectations.

### 3. Run the Script

```bash
python instagram_follow_checker.py
```

---

## Output

* Lists usernames of accounts you follow that **do not follow you back**.
* If all users follow you back, the script will notify you with a congratulatory message.

---

## Troubleshooting

* **File Not Found**: Ensure the JSON files exist in the script directory with the correct filenames.
* **JSON Structure Issues**: Instagram’s export format may vary. Verify the JSON files contain the expected nested username fields.
* If you encounter errors, please inspect the JSON data or adapt the script accordingly.

---

## Contributing

Feel free to fork the repo, make improvements, and submit pull requests. Issues and suggestions are welcome!
