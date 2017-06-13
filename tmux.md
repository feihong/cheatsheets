## Commands

| **Command** | **Description** |
|----------|----------|
| `tmux a` | Reattach |
| `tmux d` | Detach |
| `prefix kill-session` | Kill session |
| `prefix c` | Create window |
| `prefix ,` | Rename window |

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
