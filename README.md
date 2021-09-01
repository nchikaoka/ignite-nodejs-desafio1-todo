# To-do application using Node.js

## Simple application developed for Rocketseat's Ignite Node.js Trail - Chapter I Challenge.

# Features implemented:

- Create a user with `name`and `username`;
- Create new _todo_;
- Modify the `title`and `deadline` of an already existing _todo_;
- Set a _todo_ as _done_;
- Delete a _todo_

# During the development of this application, I practiced the following topics of Node.js:

- Build routes;
- Create and use middleware;
- REST request parameters;
- Request testing with Insomnia;
- Troubleshooting

# Routes created:
- post `/users`  
  the route shall receive a `name`and a `username` as body parameters. It returns the object of the created user and the status 201.

- GET `/todos`  
  the route shall receive, via request header, a `username`. It returns the todo list of the user and status 200.

- POST `/todos`  
  the route shall receive a `title`and a `deadline` as body parameters and a `username` via request header. A new task is created in the user's todo list and the new task is returned with status 201.

- PUT `/todos/:id`  
  the route shall receive a `title`and a `deadline` as body parameters, a `username`via request header and the task id `id` as route parameter. The task with id equal to `id` in the user todo list will have the `title`and `deadline` edited. The edited task is returned with status 201.

- PÀTCH `/todos/:id/done`  
  the route shall receive a `id` via route params and `username` via request header. The property `done` of the task is set to `done`. The task is then returned with status 201.

- DELETE `/todos/:id`  
  the route shall receive a `id`via route params and `username` via request header. The task is deleted from the user's todo list. The status 204 is returned.
