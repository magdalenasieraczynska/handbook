
# Instalacja środowiska dev na MacOS Moyave

* sprawdźmy czy mamy najnowszą wersję systemu jeśli nie to weźmy update
* zmiana szybkości klawiatury w menu: System Preferences (keep repeat : Fast, Delay until Repeat: Short) Trackpad (Tracking speed: Fast) i myszy
* zmiana w Terminal > Preferences > Profile terminala na Homebrew (czarny z zielonymi czcionkami), window 100x30, font 14,  zapis: Default
* instalacja update-ow w AppStore
* instalacja XCode, nie trzeba instlaować XCode z AppStore wystarczy:
```
xcode-select --install
```

* instalacja Homebrew

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
```

* inne
brew install mc
