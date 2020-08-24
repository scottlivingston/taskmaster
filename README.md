# Taskmaster

Taskmaster is an electron app to keep track of tasks you need to do.

## Features

- global hotkey for quickly adding new tasks
- main window to manage all tasks
- adding arbitrary columns of data?
- native notifications
- automatic task duration
  - keeps track of how long your current tasks will take to complete
  - pomodoro timer style task completion system
  - can i gamify this at all?
- google calendar integration to schedule tasks as meetings automatically

## Data

### Task

```scala
case class Task(
    id: Long,
    body: String,
    dueDate: DateTime,
    reminders?,
    startTime: DateTime,
    endTime: DateTime,
    status: Status,
    tags: List[String],
    color: String,
    duration: Duration,
    
)
```

