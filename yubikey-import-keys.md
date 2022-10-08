1. Plug in your Yubikey.
2. Run `gpg --card-edit`.
3. Enter `fetch` to download the keys from the Yubikey.
4. Enter `quit` to exit the gpg card editor.
5. Confirm the keys have been linked by running `gpg --list-secret-keys --keyid-format=long`.
6. Now you need to trust the keys. Run `gpg --edit-key <key-id>` for each key you want to trust.
7. Enter `trust` to set the trust level.
8. Choose `5` to set the trust level to ultimate.
9. Enter `quit` to exit the gpg key editor.