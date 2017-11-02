brew (homebrew - mac installer)

Brew already provide a command to uninstall it self:
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall)"
If you failed to run this command due to permission (like run as second user), add sudo
Then you can install again:
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"