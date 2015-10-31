To check your current default shell:
`$ echo $SHELL`

If it shows `/bin/bash` , then your current default shell is `bash`

Now to change the default shell (let us say to `zsh`), first you have to check if zsh (or any other which you need to make your default) is in your authorized shells list (`/etc/shells`).

The correct way for a user to change his or her shell is via the `chsh` command.

`chsh` stands for change shell, and does exactly what the name suggests.

You can supply the shell name with the -s argument:
`$ chsh -s /bin/zsh <username>`
where `<username>` is the user for which you want to apply the default shell.

OR, it can also work without showing the username:
`$ chsh -s /bin/zsh`