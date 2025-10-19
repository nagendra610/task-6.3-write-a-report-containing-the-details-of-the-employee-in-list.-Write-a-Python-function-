# task-6.3-write-a-report-containing-the-details-of-the-employee-in-list.-Write-a-Python-function-
You need to write a report containing the details (Name, departments) of the employee in list.
def write_employee_report(filename):
    employees = [
        {"name": "Alice", "department": "HR"},
        {"name": "Bob", "department": "Engineering"},
        {"name": "Charlie", "department": "Finance"}
    ]

    with open(filename, "w") as file:
        for employee in employees:
            line = f"Name: {employee['name']}, Department: {employee['department']}\n"
            file.write(line)
