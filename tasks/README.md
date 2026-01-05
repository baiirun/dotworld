# Tasks

This directory is used by the `tasks` CLI for agent task management.

## Setup

Install the CLI from [dotworld-tasks](https://github.com/baiirun/dotworld-tasks), then:

```bash
tasks init
```

This creates `tasks.db` in this directory.

## Usage

```bash
tasks add "Build auth system"     # create task
tasks ready                       # see what's unblocked
tasks start <id>                  # claim a task
tasks done <id>                   # complete it
```

See the tasks-go repo for full documentation.
