# mikoshell
Simple Shell for Paramiko

```
import paramiko
#
from mikoshell import Shell, ShellPrompt

with Shell(paramiko.Channel(), ShellPrompt()) as shell:
    print shell.command('show version')

```
