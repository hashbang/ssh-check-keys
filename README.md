# test_authorized_keys
Standalone project for auditing the security and tsting valid form of authorized_key lines or files.

Should initially test for:

* valid form (including command= lines etc)
* small key sizes
* keys impacted by 2008 compromized randomness bug in openssh

should take one or more keys via stdin or a filename. exit 0 if all checks pass
