# Elixir Enum.each and Process.exit

This repository demonstrates a potential issue in Elixir when combining `Enum.each` with `Process.exit`.  The example code shows how a process can be unexpectedly terminated within the loop, and how to avoid this issue.  Using `Enum.each` with functions that might terminate the process is not recommended.  Better approaches such as `Enum.map` or `Enum.reduce` are safer for handling potential exit conditions.

See `bug.exs` for the buggy code and `bugSolution.exs` for the corrected version.