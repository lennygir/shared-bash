 # Shared-bash

Utilities for bash

## Install a script

Change `<script>` by the name of the script you want to install

```bash
SCRIPT=<script> && cd /usr/bin && { sudo curl -O https://raw.githubusercontent.com/lennygir/shared-bash/master/$SCRIPT ; cd -; } && cd /usr/share/man/man1/ && { sudo curl -O https://raw.githubusercontent.com/lennygir/shared-bash/master/$SCRIPT.1.gz ; cd -; } && sudo chmod +x /usr/bin/$SCRIPT
```

NOTE : your password may be asked because it adds the script into the /usr/bin folder (which is a protected folder)

## usable scripts : 
- gpush : Add, commit and push to a specific branch in one command
