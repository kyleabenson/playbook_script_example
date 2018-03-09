This is a simple playbook and script to highlight how Ansible handles scripts.

It highlights how Ansible wraps around a script and how stderr is included with stdout.

To higlight this, in python run:
```
$ python python_simple 2> /dev/null
Hello from Kyles-MacBook-Pro.local
This script ran in /Users/kylebenson/Documents/Work/playbook_script_example
$ python python_simple 1> /dev/null
****Example of standard err****
```

Then run via ansible-playbook to observe differences
