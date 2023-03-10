# task-manager-js

#### Tiny To-Do-List-type task manager created using basic HTML/CSS/JS on the front side, and Node.js, paired with Express.js and MongoDB on the backend.

##### Features:
1. Task creation
2. Task deletion
3. Editing/patching
4. Saving information to the database

##### To setup, run `npm install` and create the `.env` file, filling up the `MONGO_URI` and `SERVER_PORT` fields.

##### Run it using the `npm start` for production, and `npm run dev` for the development environment, supported by Nodemon.

---

#### It does the following API calls:

Method | URL | Function
--- | --- | ---
| `GET:` | `/api/v1/tasks` | Retrieves a list of all tasks from the server
| `GET:` | `/api/v1/tasks/:ID` | Retrieves a specific task from the server 
| `POST:` | `/api/v1/tasks` | Creates a new task 
| `PATCH:` | `/api/v1/tasks/:ID` | Updates a specific task on the server 
| `DELETE:` | `/api/v1/tasks/:ID` | Deletes a specific task 
---
#### The MongoDB Schema is as follows:

```
  {
    _id: "ID, default",
    name: "Task Content, String",
    completed: true/false, Boolean
  }
```
