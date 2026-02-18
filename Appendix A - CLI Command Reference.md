# Appendix A — CLI Command Reference

Quick reference for `openclaw` CLI commands.

---

## Gateway

```bash
openclaw gateway stop          # Stop the agent process
openclaw gateway start         # Start the agent process
openclaw gateway restart       # Restart the agent process
openclaw gateway status        # Check if gateway is running
```

## Configuration

```bash
# Gateway binding
openclaw config set gateway.bind "127.0.0.1"

# Docker sandbox
openclaw config set agents.defaults.sandbox.mode "all"
openclaw config set agents.defaults.sandbox.scope "session"
openclaw config set agents.defaults.sandbox.workspaceAccess "ro"
openclaw config set agents.defaults.sandbox.docker.network "none"
openclaw config set agents.defaults.sandbox.docker.memory "512m"
openclaw config set agents.defaults.sandbox.docker.cpus 1
openclaw config set agents.defaults.sandbox.docker.pidsLimit 100

# Tool policy
openclaw config set tools.deny '["browser", "exec", "process", "apply_patch", "write", "edit"]'
openclaw config set tools.allow '["read", "web_search", "web_fetch", "sessions_list", "sessions_history"]'
openclaw config set tools.elevated.enabled false
```

## Sandbox

```bash
openclaw sandbox explain       # Show current sandbox configuration
openclaw sandbox set [options] # Modify sandbox settings
```

## Sessions

```bash
openclaw sessions list                                    # List active sessions
openclaw sessions send --target <session_key> --message "/new"  # Reset a session
```

## Security

```bash
openclaw security audit        # Run built-in security audit
```

## Models & Auth

```bash
openclaw models auth add       # Add/rotate API key for a provider
openclaw status --usage        # Check current API usage across providers
```

## Credential Rotation

```bash
# Rotate an API key
openclaw models auth add       # Choose provider, paste new key
openclaw gateway restart       # Apply the new key

# Rotate Telegram bot token
# 1. Go to @BotFather on Telegram
# 2. Send /revoke to get a new token
# 3. Update in openclaw config
openclaw gateway restart
```

## Plugins

```bash
openclaw plugins install <name>   # Install a plugin
openclaw plugins list              # List installed plugins
```
