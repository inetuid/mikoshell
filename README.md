# mikoshell
Simple Shell for Paramiko

```
import paramiko
#
from mikoshell import Shell, ShellPrompt

ssh_client = paramiko.SSHClient()
ssh_client.connect('127.0.0.1', username='testuser', password='testpass')

shell_prompt = ShellPrompt('My Prompt>')
shell_prompt.add_prompt('My Prompt (2)>')

with Shell.from_transport(ssh_client.get_transport(), shell_prompt) as shell:
    print shell.command(command_a)
    print shell.command(command_b)

```
