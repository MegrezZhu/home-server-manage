This is the playbooks for managing my own home network services.

Commands to use:

```sh
ansible-playbook all.yaml -i inventory -J;
```

Some credentials are encrypted in this repo. (Note for myself: password of it is stored in 1PassWord).

For development:

```bash
python3 -m venv .venv;
source .venv/bin/activate;
pip install -r requirements.txt;
```

References

- [1Password integration in WSL](https://gist.github.com/WillianTomaz/a972f544cc201d3fbc8cd1f6aeccef51)
