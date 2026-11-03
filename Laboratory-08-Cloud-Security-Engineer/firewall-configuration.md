# Firewall Configuration Documentation

## Executed Security Commands

**The command used to allow SSH**
   ```bash
   sudo ufw allow ssh
```

**The commands used to set the Default Deny policy**
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

**The command used to allow Port 8080**
```bash
sudo ufw allow 8080/tcp
```
**A brief 1-sentence explanation of what would happen if you ran sudo ufw enable before running sudo
ufw allow ssh.**

If you run sudo ufw enable before running sudo ufw allow ssh, UFW immediately blocks all incoming traffic on Port 22. This instantly drops your active SSH session and permanently locks you out of the server, leaving you with no way back in unless you reset the instance.
