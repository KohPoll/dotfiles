copy and modify from https://github.com/mathiasbynens/dotfiles, thanks a lot.

brew(http://brew.sh/)

Homebrew installs packages to their own directory and then symlinks their files into /usr/local.

```
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
```


pip(https://pypi.python.org/pypi/pip)
```
cd dotfiles/init/pip-1.5.4
sudo python setup.py install

sudo pip install virtualenv
sudo pip install virtualenvwrapper


mysql:

brew install mysql

auto start:
```
To have launchd start mysql at login:
    ln -sfv /usr/local/opt/mysql/*.plist ~/Library/LaunchAgents
Then to load mysql now:
    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
```
