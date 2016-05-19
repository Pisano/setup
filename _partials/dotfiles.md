## Dotfiles (Standard configuration)

Hackers love to refine and polish their shell and tools. We'll start with a default configuration stored on GitHub. As your configuration is personal, you need your own repository storing it, so you first need to fork it to your GitHub account.

:arrow_right: [Click here to **fork**](https://github.com/Pisano/dotfiles/fork) the `Pisano/dotfiles` repository to your account. Forking means that it will create a new repo in your GitHub account, identical to the original one. You'll have a new repository on your GitHub account, `your_github_username/dotfiles`. We need to fork because each of you will need to put specific information (e.g. your name) in those files.

Open your terminal. **Don't blindly copy paste this line**, replace `replace_this_with_your_github_username` with *your*
own github usernickname.

```bash
export GITHUB_USERNAME=replace_this_with_your_github_username
# Example:
#   export GITHUB_USERNAME=omurturan
```

Now copy/paste this very long link to your terminal. Do **not** change this one.

```bash
mkdir -p ~/code/$GITHUB_USERNAME && cd $_ && git clone git@github.com:$GITHUB_USERNAME/dotfiles.git && cd dotfiles
```

Run the `dotfiles` installer.

```bash
zsh install.sh
```

Then run the git installer. It will **prompt** you for your name and your email.

```bash
zsh git_setup.sh
```

Please now **quit** all your opened terminal windows.

### Sublime Text auto-configuration

In the terminal, type this:

```bash
stt
```

It will **open Sublime Text in the context of your current folder**. That's how we'll use it.
 **Wait a bit** for additional packages to be automatically installed (New tabs with text will automatically open, containing
 documentation for each new package installed). To check if plugins are installed,
 open the Command Palette (`⌘` + `⇧` + `P` on OSX, `Ctrl` + `⇧` + `P` on Linux), type in `Packlist` and then `Enter`, you should
 see a couple of packages installed (like [Emmet](http://emmet.io/)). If you are not sure, ask a teacher.


