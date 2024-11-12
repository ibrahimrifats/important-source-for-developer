
# SSH Key Setup and Server Connection

## Step 1: Create an SSH Key
Generate a new SSH key by running this command in your terminal. Replace `"your-email@example.com"` with your own email:

```bash
ssh-keygen -t rsa -b 4096 -C "your-email@example.com"
```

- Follow the prompts to choose a save location (press Enter to accept the default).
- Optionally, add a passphrase for additional security.

## Step 2: Connect to Your Server
After creating the SSH key, use the command below to connect to your server. Replace `/path/to/your/id_rsa` with the actual path to your private key file, and use the correct **username** and **hostname** provided by your server.

```bash
ssh -i /path/to/your/id_rsa username@hostname
```

### Example:
- **Hostname**: `ssh.example.com`
- **Username**: `user@example.com`

```bash
ssh -i /home/your-username/.ssh/id_rsa user@example.com@ssh.example.com
```

Now you should be connected to your server using SSH!
