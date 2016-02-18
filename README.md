# ssh-check-keys

Standalone project for auditing the security and tsting valid form of authorized_key lines or files. 

Should initially test for:

* valid form (including command= lines etc)
* small key sizes
* keys impacted by 2008 compromized randomness bug in openssh

Should take one or more keys via stdin or a filename. exit 0 if all checks pass
If run with no stdin or arguments, will check the .ssh/authorized_keys{,.d/*} for the current user.

Prefer development in something common that outputs a static binary such as C or Go
