# Ansible Role: Install python by pyenv

Ansible Role: Install python by pyenv

## Dependencies

Before execute thie playbook, you should execute the playbooks below.

- [gano2018.ansible_anyenv](https://github.com/gano2018/ansible_anyenv)

## Role Variables

- python_pyenv_install_dir (defined at `defaults/main.yml`)

  The variable `python_pyenv_install_dir` is where pyenv is installed.
  The default value is `/opt/anyenv/envs/pyenv`.

  The variable is define as `{{ anyenv_root | default '/opt/anyenv'}}//envs/pyenv`, so you only define `anyenv_root` if you want to change the default value.

- python_version (defined at `defaults/main.yml`)

  The variable `python_version` is the version you want to install.
  The default value is `2.7.15`. If you do not define, version `2.7.15` will be installed.

- python_required_libraries (defined at `vars/*.yml`)

  The libraries required to install python. The values are change by os type.
