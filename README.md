# 📧 Email Extractor

A lightweight Python script that scans a text file and extracts all valid email addresses, saving them to a separate output file.

## Features

- Extracts all valid email addresses from any `.txt` file
- Removes duplicate emails automatically
- Saves results to a clean output file
- Handles missing input file with a clear error message

## Requirements

- Python 3.x
- No external libraries required (uses built-in `re` module)

## Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/nasirbhatti14/CodeAlpha_task_automation.git
   ```

2. **Add your text file**  
   Place your text file in the project directory and name it `data.txt`, or update the filename in the script.

3. **Run the script**
   ```bash
   python task_automation.py
   ```

4. **Check the output**  
   Extracted emails will be saved to `emails.txt` in the same directory.

## Example

**Input (`data.txt`):**
```
Contact us at support@example.com or sales@company.org
For billing, reach out to billing@example.com
```

**Output (`emails.txt`):**
```
support@example.com
sales@company.org
billing@example.com
```

## How It Works

The script uses a regular expression pattern to match valid email addresses:

```
[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}
```

This matches standard email formats including subdomains and various TLDs.

## Project Structure

```
email-extractor/
│
├── email_extractor.py   # Main script
├── data.txt             # Input file (add your own)
├── emails.txt           # Output file (auto-generated)
└── README.md
```

## License

This project is open source and available under the [MIT License](LICENSE).
