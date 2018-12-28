rubygems_environment
=========

Set `rubygems_environment` fact storing the result of `gem
environment` command.

And these two facts are defined.

- `rubygems_executable_directory`
- `rubygems_executable_path`

Requirements
------------

The `gem` command needs to run on the remote machine.  If the name of
the `gem` command is different, it must be set in the
`rubygems_command` variable.

Role Variables
--------------

| Variable | Default | Description |
|----------|---------|-------------|
|`rubygems_command`|`gem`|rubygems command|
|`rubygems_show_environment`|`false`|display contents of `rubygems_environment` fact on the console.|

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - role: y10k.rubygems_environment
```

License
-------

BSD
