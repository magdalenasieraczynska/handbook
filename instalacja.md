
# Instalacja środowiska dev na MacOS Moyave

* sprawdźmy czy mamy najnowszą wersję systemu jeśli nie to weźmy update
* zmiana szybkości klawiatury w menu: System Preferences (keep repeat : Fast, Delay until Repeat: Short) Trackpad (Tracking speed: Fast) i myszy
* zmiana w Terminal > Preferences > Profile terminala na Homebrew (czarny z zielonymi czcionkami), window 100x30, font 14,  zapis: Default
* instalacja update-ow w AppStore
* instalacja XCode, nie trzeba instlaować XCode z AppStore wystarczy:
```
xcode-select --install
```

* instalacja Homebrew https://brew.sh/

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor
brew update
```


* instalacja języka Ruby

```
rbenv install -l #list ruby versions
rbenv install 2.5.2 #uwaga tu nalezy sprawdzic jaka jest najwieksza wersja 
rbenv global 2.5.2

echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
source ~/.bash_profile

# w nowym oknie termala powinna byc juz nowa wersja rubiego
ruby -v

```

* inne
brew install mc
