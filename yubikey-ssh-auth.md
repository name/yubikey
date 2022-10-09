1. Install GPG4Win and PuTTY.
2. Insert Yubikey.
3. Open a command prompt (e.g. by searching for cmd.exe).
4. Run gpg --version. Put the file gpg-agent.conf from above into the home directory listed.
5. Run gpg-connect-agent KILLAGENT /bye.
6. Run gpg --card-status. It should print information about your Yubikey.
7. Thats it! You can now use your Yubikey for authentication using PuTTY.


gpg-agent.conf File contents:


enable-putty-support