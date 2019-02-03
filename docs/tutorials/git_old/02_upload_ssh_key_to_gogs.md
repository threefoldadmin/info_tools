# How to upload SSH Key to GOGs



1. Go to `Your Settings`
![gogs settings location]( https://docs.grid.tf/dividi/efika_tools_tutorials/raw/master/git/images/gogs_settings_location.png)

2. Go to `SSH Keys` section and press `Add Key` button.
![gogs settings sshkey location]( https://docs.grid.tf/dividi/efika_tools_tutorials/raw/master/git/images/gogs_settings_sshkey_location.png)

3. Locate your SSH Key.
If you do not have it yet, [generate it](https://docs.grid.tf/dividi/efika_tools_tutorials/src/master/git/01_ssh_key_generation_osx.md)
Your public key is saved to the `id_rsa.pub` file and is the key you can upload to remote resources or share with anyone you need. You can save this key to the clipboard by running this:
```
cat ~/.ssh/id_rsa.pub
```   
Copy it to the clipboard. Make sure you do not take any unnecessary text or spaces.

4. Add any name as you like and paste your public key to the `Content` field. You should have it in your clipboard after the previous step.
![gogs_settings_sshkey_adding]( https://docs.grid.tf/dividi/efika_tools_tutorials/raw/master/git/images/gogs_settings_sshkey_adding.png)

5. Press `Add Key` button.

Done!
