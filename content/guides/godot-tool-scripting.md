---
title: Godot Tool Scripting
layout: page
published: true
---

# Godot Tool Scripting

## Godot Command Palatte

How to write a command that can be run from the Godot Command Palatte:

```gd
var command_palette = EditorInterface.get_command_palette()
# external_command is a function that will be called with the command is executed.
var command_callable = Callable(self, "external_command").bind(arguments)
command_palette.add_command("command", "test/command",command_callable)
```

---

Written by [Jonathan Lewis](https://www.linkedin.com/in/jonathan-david-lewis/)

Please reach out if you have any questions or suggestions for improvements.