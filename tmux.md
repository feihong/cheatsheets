## Commands

| **Command line** | **Description** |
|----------|----------|
| `tmux ls` | list sessions |
| `tmux a` | Reattach to last session |
| `tmux new -s foo` | Create new session named foo |
| `tmux a -t foo` | Attach to session named foo |

Prefix, by default, is ^b.

| **Key bindings** | **Description** |
|----------|----------|
| `prefix d` | Detach |
| `prefix kill-session` | Kill session |
| `prefix c` | Create window |
| `prefix ,` | Rename window |
| `prefix [` | Enter scroll mode. You can use arrow and page keys to scroll. Press q to quit. |

## Sample tmuxinator file

```yaml
# ~/.tmuxinator/project.yml

name: project
root: ~/work/project

# Runs in each window and pane before window/pane specific commands. Useful for
# setting up interpreter versions.
# pre_window: rbenv shell 2.0.0-p247

windows:
  - services:
      layout: even-vertical
      panes:
        - /usr/local/sbin/rabbitmq-server
        - webpack:
          - cd client
          - invoke clientserver
        - admin:
          - workon awesome
          - cd admin
          - ./manage.py runserver
  - tasks:
    - workon tasks
    - celery -A tasks worker --loglevel=info
```

## Sources

- http://www.dayid.org/comp/tm.html
- http://hyperpolyglot.org/multiplexers
