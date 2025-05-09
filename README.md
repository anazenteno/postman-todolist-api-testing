# ✅ Todo List API Testing with Postman

This project contains API tests created in Postman while practicing with a sample Todo List application.

## 🧰 Tools Used
- Postman (Collections & Tests)
- Newman (Command-line test runner)
- Sample API: Todo List (local or public)

## 🧪 What Was Tested
- Set up the test environment
- Implement the following automated tests:
  - Create Task: Check that a new task can be created using POST /tasks.
  - List Tasks: Check that tasks can be retrieved using GET /tasks.
  - Update Task: Check that an existing task can be updated using PUT /tasks/{id}.
  - Delete Task: Check that an existing task can be deleted using DELETE /tasks/{id}
  - Data Validation: Check that an error message appears when trying to create a task with invalid data.
- Add proper assertions to each test to verify the response.
- Set up an automated test report to show the results clearly.

## 🚀 How to Run

### Using Postman
1. Import the collection from `/collections/todolist_collection.json`
2. Set up the environment from `/environments/local_env.json` (if used)
3. Run each request manually or use the Collection Runner
4. Set up an automated test report to show the results clearly.
5. More step [Installation & Setup instructions](./HOW_TO_RUN.md)
