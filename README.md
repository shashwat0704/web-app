# Task Management Web Application

This web application helps students manage tasks for different courses. It provides endpoints to retrieve, add, update, and delete tasks associated with specific courses.

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose

## API Endpoints
### Retrieve Tasks
GET /courses/:courseId/tasks
Retrieve tasks associated with a specific course.

### Add Task
POST /courses/:courseId/tasks
Add a new task for a specific course.
Request body example:
/courses/React/tasks

```json
{
    "taskName" : "Week 7",
    "description": "Complete it by 12th March 2024",
    "dueDate" : "12-03-2024"
}```

### Update Task
PUT /courses/tasks/:taskId
Update an existing task by ID.
Request body example:
/courses/tasks/5e896fadbebaabdce4

```json
{
  "taskName": "Updated Assignment",
  "description": "Updated description",
  "dueDate": "2024-03-15"
}```

### Delete Task
DELETE /courses/tasks/:taskId
Delete a task ID
