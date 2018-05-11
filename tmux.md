# tmux Commands and Shortcuts

### Commands

```sh
# Create Session
$ tmux                                  # create a session
$ tmux new -s SESSION_NAME              # create a session and put a name to it

# Detach Session
$ tmux detach                           # detach the current session, and can attach again

# Quit Session
$ exit                                  # quit a session, and cannot return the session
$ logout                                # type logout can also leave a session

# Attach Session
$ tmux attach                           # attach a session
$ tmux attach -t SESSION_NAME           # attach a specific session

# Kill Session
$ tmux kill-server                      # kill the server (all sessions)
$ tmux kill-session -t SESSION_NAME     # kill a specific session

# List Sessions
$ tmux ls                               # list all sessions
```

---

### Shortcuts

| Description | Shortcuts (used inside tmux) |
| ------ | ------ |
| Create session | **Ctrl+b, :new<CR>** |
| Create window | **Ctrl+b, c** |
| **Create vertical pane** | **Ctrl+b, "** |
| **Create horizontal pane** | **Ctrl+b, %** |
| Swap session | **Ctrl+b, s** |
| Swap next window | **Ctrl+b, n** |
| Swap previous window | **Ctrl+b, p** |
| **Swap pane** | **Ctrl+b, Arrow_Keys** |
| List session | **Ctrl+b, s** |
| List window | **Ctrl+b, w** |
| Rename session | **Ctrl+b, $** |
| Rename window | **Ctrl+b, ,** |
| Kill session | **Ctrl+b, :kill-session<CR>** |
| Kill window | **Ctrl+b, &** |
| **Kill pane** | **Ctrl+d** |
| Detach session | **Ctrl+b, d** |
| Check all shortcuts | **Ctrl+b, ?** |
