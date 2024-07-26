Step 1 Generating public/private rsa key pair.

$ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
You'll be asked to confirm where to save the SSH key and what passphrase you want to use.

Step 2 Add your key to the ssh-agent

Ensure ssh-agent is enabled

$eval "$(ssh-agent -s)"

Add your SSH key to the ssh-agent:

$ssh-add ~/.ssh/id_rsa