# mikoshell
Simple Shell for Paramiko

```
from mikoshell import Shell, ShellPrompt

with Shell(paramiko.Channel(), ShellPrompt()) as shell:
    print shell.command('show version')

```
