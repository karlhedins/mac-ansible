mac-ansible
===========

I use this project to configure my macOS the way I like it. That way I can wipe
and re-install with less effort.

This project was forked from Adam Johnson's [mac-ansible](https://github.com/adamchainz/mac-ansible) repo.
Here's his original blog post describing his setup:
[blog post](https://adamj.eu/tech/2019/03/20/how-i-provision-my-macbook-with-ansible/).

Getting Started
---------------

1. Install [homebrew](http://brew.sh/) with the command from the site
2. `brew install pyenv`
3. `pyenv install <latest_python_version>` (Check playbook up to date)
4. Make sure pyenv's python on path (it will be after my shell settings are in place from playbook)
5. `python -m venv venv`
6. `source venv/bin/activate`
5. `pip install ansible` (always the best way to install Ansible)
6. Then `./playbook.yml`

Most tasks are tagged. To run tasks with a specific tag, for instance brew, run:

```bash
ansible-playbook playbook.yml --tags "brew"
```

Things currently installed manually
---------------
- [Fira Code font](https://github.com/tonsky/FiraCode)

Fork! Copy! Adapt!
------------------

This is distributed under the Unlicense so you can do whatever you want with
it, see LICENSE.
