# Macbook

Let's try to use ansible to make your mac ready to rock.

## Install

```
git clone https://github.com/lktslionel/macbook.git $HOME/.macbook
```

## Usage

Run the following command to start the setup process

```
$HOME/.macbook/macbook-manager
```

You can customize the setup process to your conviniance by defining an ansible role.
When that's done, you registry your role in the `[macbook-manager](https://github.com/lktslionel/macbook/blob/master/macbook-manager)`.

```bash
#!/usr/bin/env ansible-playbook

---
- hosts: localhost
  connection: local
  roles:
    - role: dev
#   - role: <YOUR_NEW_ROLE> 
```

## Acknowledgments

Great thanks to [@bennylope](https://github.com/bennylope) for the inspiration.


## License

MIT License

