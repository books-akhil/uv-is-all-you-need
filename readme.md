# UV is all you need

UV is a modern python package manager which is extremely fast. Its global cache helps in not duplicating existing packages in in other virtual envs. When we init a project with uv, it creates a 
pyproject.toml file and uv.lock file, which creates all the magic.

[UV Documentation](https://docs.astral.sh/uv/getting-started/)

## Basic UV commands

- To initialise a new project
```shell
uv init project-name
```

- To initialise in existing project. Navigate to the folder
```shell
uv init
```

- To update the project
```shell
uv sync
```

- Add Dependency
```shell
uv add module
```

- Visualise the dependencies
```shell
uv tree
```

- Run the code
```shell
uv run main.py
```

- Install tools
```shell
uv tool install ruff
```
This creates a global installation
```shell
ruff check
```

- To temp run a tool without install
```shell
uv tool run ruff
```
(or)
```shell
uvx ruff
```

- To list all tools
```shell
uv tool list
```

## Workspaces

Add a project in another project

