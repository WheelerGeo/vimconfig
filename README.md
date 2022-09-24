#install vim-plug
```
mkdir -p ~/.vim/autoload/
mv plug.vim ~/.vim/autoload/
```

#install powerline font
```
sudo apt install fonts-powerline
```

#update nodejs to latest(optional)
```
curl -sL https://deb.nodesource.com/setup_16.x -o /tmp/nodesource_setup.sh
sudo bash /tmp/nodesource_setup.sh
sudo apt update
sudo apt install nodejs
```

#update vim to latest(optional)
```
sudo apt-get install software-properties-common
sudo apt update
sudo apt install vim
```

#update Coc config to open auto-complete
```
1. vim input
:CocConfig
2. modify coc-settings.json
{
    "languageserver": {
	"golang": {
	    "command": "gopls",
	    "rootPatterns": ["go.mod", ".vim/", ".git/", ".hg/"],
	    "filetypes": ["go"]
	}
    }
}
3. CocInstall
```
