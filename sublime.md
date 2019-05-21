# Sublime

* wersja 3176 ostatna bez git (szybsza): https://download.sublimetext.com/Sublime%20Text%20Build%203176.dmg
* wersja aktualna: https://www.sublimetext.com/3 

## Skrót subl

```
ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl
subl .
```

## Odpalanie Sublime z przeglądarki (podczas będów Railsów)

aby linki po bledach w przegladarce na DEV byly klikalne trzeba przeniesc do Applications apke z Subl.app.zip (jest w katalogu extensions) i uruchomic (dziala z Sublime 3 i 2) (apka sie od razu zamknie ale i tak linki zaczną działać - sprawdzon na Mac Book Air 2015.04.10 i Mac Book PRO 2015)

## Formatowanie kodu

na pliku danego formatu (*.rb, *.js, *.erb itp) wybieramy Sublime Text > Preferences > Settings
```
	"tab_size": 2,
	"translate_tabs_to_spaces": true,
	"trim_trailing_white_space_on_save": true,

np:
```
{
	"color_scheme": "Packages/Color Scheme - Default/Monokai.tmTheme",
	"font_size": 11,
	"theme": "Default.sublime-theme",
	"update_check": false,
	
	"tab_size": 2,
	"translate_tabs_to_spaces": true,
	"trim_trailing_white_space_on_save": true,
}
```

## Edytor kodu

Używamy edytora Sublime 3. Skróty, które warto znać:
* wyszukiwanie pliku po nazwie: CMD + T
* wyszukiwanie metody w pliku: CMD + R
* przechodzenie do linii : CMD + R
* wyszukiwanie w całym projekcie : SHIFT + CMD + F
* uruchanianie pluginów: CMD + SHIFT + P (lub instalacja nowych - trzeba wpisać "install...")


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


