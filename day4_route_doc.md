Task resources routing:

1. List all the tasks

Request:

GET /tasks

WorkFlow:
Rails send the request to the TaskController and index operation is perform.

2. Display one task:

Request:
Get /tasks/:id
i.e
/task/3

Workflow:
Rails send the request to the TaskController and then show action is perform and it shows the task 5 details.

3. New Task

   Request:
   GET /tasks/new

   Workflow:
   Rails send the request to the TaskController and new operation is perform in which new form is open to the user to enter the new task.

4. Create New Task:

Request:
POST /tasks

Workflow:
Rails send the request to the TaskController and create operation is perform in which user can create a new task and save it to the database storage.

5. Edit task through form:

Request:

GET /task/:id/edit

WorkFlow:
Rails sent the request to the TaskController and edit action is perform in which user can edit the task through the form.

6. Update the task:

Request:

PATCH /tasks/:id

WorkFlow:
Rails send the request to the TaskController and update operation is perform in which user can update the specific task.

7. Delete Task:

Request:

DELETE /tasks/:id

WorkFlow:
Rails send the request to the TaskController and destroy operation is perform in which user can delete/destory the specific task.
