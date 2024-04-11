# Zed config

This is a minimalist setup of Zed

- disabled Co-pilot
- disabled Collaboration
- disabled Assistant


Setting up your workflow:

CMD + SHIFT + C = Open Local Task 

<details>
  
  <summary>setup task.json e.g. add `leptosfmt` </summary>
  
<code>
[
  {
    "label": "leptos fmt",
    "command": "leptosfmt src/",
    "env": { "RUST_LOG": "leptosfmt=debug" },
    // "env": {  },
    // Current working directory to spawn the command into, defaults to current project root.
    //"cwd": "/path/to/working/directory",
    // Whether to use a new terminal tab or reuse the existing one to spawn the process, defaults to `false`.
    "use_new_terminal": false,
    // Whether to allow multiple instances of the same task to be run, or rather wait for the existing ones to finish, defaults to `false`.
    "allow_concurrent_runs": false,
    // What to do with the terminal pane and tab, after the command was started:
    // * `always` — always show the terminal pane, add and focus the corresponding task's tab in it (default)
    // * `never` — avoid changing current terminal pane focus, but still add/reuse the task's tab there
    "reveal": "always"
  }
]

</code>

</details>

CMD + SHIFT + R = Choose a Task to Run

CMD + R - Triggers Task Re-run


For Running Test:

1. Initially Press CMD + SHIFT + R - Task Spawn
2. Choose: Rust Test Current Function
3. Then Press CMD + R , to re run test


## TODO:
- Implement Cargo runner

