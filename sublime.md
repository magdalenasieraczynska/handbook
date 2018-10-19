# Sublime

http://www.sublimetext.com/3

```
ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl
subl .
```

Sublime > Preferences > Color Scheme > Mac Classic

aby linki po bledach w przegladarce na DEV byly klikalne trzeba przeniesc do Applications apke z Subl.app.zip i uruchomic (dziala z Sublime 3 i 2) (apka sie od razu zamknie ale i tak linki zaczną działać - sprawdzon na Mac Book Air 2015.04.10 i Mac Book PRO 2015)

## Pluginy do Sublime

Formatowanie kodu Ruby i ERB:
```
gem install 'htmlbeautifier'
```

instalacja https://packagecontrol.io/packages/BeautifyRuby
* pozniej najechanie w erb/rb i Command+Shift+P i wybranie BeautifyRuby
* uwaga u mnie trzeba było przestawić wersję rubiego: "ruby": "~/.rvm/bin/…….",

handlebars plugin do sublime
https://github.com/daaain/Handlebars/
```
cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages
git clone https://github.com/daaain/Handlebars.git Handlebars
```

* https://github.com/kemayo/sublime-text-git/wiki
* https://github.com/cbumgard/GitCommitMsg


