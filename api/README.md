# API Data Exporter

## Description

This project demonstrates how to interact with a RESTful API using Python to retrieve employee data and export it into different formats (CSV and JSON). It is part of the **ALU Backend Specialization** curriculum and aims to teach students practical skills in working with APIs, handling data formats, and writing clean, modular Python code.

For a given employee ID, the script will:

- Retrieve their TODO list data from a public API.
- Display the progress of completed tasks.
- Export the data to:
  - CSV format (`USER_ID.csv`)
  - JSON format (`USER_ID.json`)

---

## Background

System administrators are evolving into Site Reliability Engineers (SREs) who use modern programming tools like Python to automate tasks and manage systems. Shell scripts can become messy and inefficient for data parsing or API interaction, making Python the ideal choice for such tasks.

---

## Learning Objectives

By completing this project, you will learn:

- What an API is and how to interact with it using HTTP requests.
- The difference between REST APIs and microservices.
- The structure and purpose of JSON and CSV formats.
- Python naming conventions and code structure following **PEP8**.
- How to build modular and readable Python scripts.

---

## Requirements

- Python 3.4.3
- Ubuntu 14.04 LTS
- Allowed editors: `vi`, `vim`, `emacs`
- Code must follow PEP8 style guidelines.
- All scripts must be executable.
- Use `requests` or `urllib` module for API calls.
- All output files must end with a new line.
- Handle potential key errors using `.get()`.
- Scripts must not execute code when imported (use `if __name__ == "__main__":`)

---

## File Structure

```bash
api/
├── 0-gather_data_from_an_API.py     # Displays TODO list progress
├── 1-export_to_CSV.py               # Exports TODO list to CSV format
├── 2-export_to_JSON.py              # Exports TODO list to JSON format
└── README.md                        # Project documentation
```

Usage
Task 0: Display TODO List Progress
$ python3 0-gather_data_from_an_API.py <EMPLOYEE_ID>


Example Output:

Employee Ervin Howell is done with tasks(8/20):
     distinctio vitae autem nihil ut molestias quo
     voluptas quo tenetur perspiciatis explicabo natus
     aliquam aut quasi
     ...

Task 1: Export to CSV
$ python3 1-export_to_CSV.py <EMPLOYEE_ID>


Output:
Creates a file named <EMPLOYEE_ID>.csv with the format:

"2","Antonette","False","suscipit repellat esse quibusdam voluptatem incidunt"
...

Task 2: Export to JSON
$ python3 2-export_to_JSON.py <EMPLOYEE_ID>

```bash
Output:
Creates a file named <EMPLOYEE_ID>.json with the structure:

{
  "2": [
    {
      "task": "suscipit repellat esse quibusdam voluptatem incidunt",
      "completed": false,
      "username": "Antonette"
    },
    ...
  ]
}
```

Author

Kenny Gael Ishimwe Gatete


## License

This project is part of the ALU curriculum and follows the guidelines and licensing terms provided by the institution.