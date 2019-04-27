
# Instalacja środowiska dev na MacOS Mojave

* sprawdźmy czy mamy najnowszą wersję systemu jeśli nie to weźmy update
* zmiana szybkości klawiatury w menu: System Preferences > Keyboard (keep repeat : Fast, Delay until Repeat: Short) Trackpad (Tracking speed: Fast) i myszy
* zmiana w Terminal > Preferences > Profile terminala na Homebrew (czarny z zielonymi czcionkami), window 100x30, font 14,  zapis: Default
* instalacja update-ow w AppStore
* instalacja XCode, nie trzeba instlaować XCode z AppStore,wystarczy:
```
xcode-select --install
```
* warto wyłączyć powiększanie pierwszej litery (System Preferences > Keyboard > Text) i ew Correct Spelling (też w tym miejscu)

## instalacja Homebrew https://brew.sh/

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor
brew update
```


## instalacja języka Ruby

```
brew install rbenv
rbenv install -l #list ruby versions
rbenv install 2.4.6 #uwaga tu nalezy sprawdzic jaka jest najwieksza wersja 
rbenv global 2.4.6

echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
source ~/.bash_profile

# w nowym oknie termala powinna byc juz nowa wersja rubiego czyli np: ruby 2.4.6p354 (2019-04-01 revision 67394) [x86_64-darwin18]
ruby -v

```

## instalacja Pow http://pow.cx/

```
brew install pow

# Create the required host directories:
mkdir -p ~/Library/Application\ Support/Pow/Hosts
ln -s ~/Library/Application\ Support/Pow/Hosts ~/.pow

# Setup port 80 forwarding and launchd agents:
sudo pow --install-system
pow --install-local

# fix do pow.cx (aby pokazywał poprawnie błędy w aplikacji zamiast "End of file reached"):

# stara wersja curl -L https://gist.githubusercontent.com/RobinDaugherty/2731f20d303e6506d451384df2189210/raw/b52e6231170b3dce39633db29634dc892751910f/pow_better_errors_fix.patch | patch ~/Library/Application\ Support/Pow/Versions/0.6.0/node_modules/nack/lib/nack/server.rb

curl -L https://gist.githubusercontent.com/RobinDaugherty/2731f20d303e6506d451384df2189210/raw/b52e6231170b3dce39633db29634dc892751910f/pow_better_errors_fix.patch | patch /usr/local/Cellar/pow/0.6.0/libexec/node_modules/nack/lib/nack/server.rb


```
projekty

```
cd
mkdir projects
mkdir projects/radgost
cd ~/.pow; ln -s ~/projects/radgost

```
teraz można odpalić:
http://radgost.test



## SSH
* warto stworzyć plik .ssh/config
* aby nie było błędów UTF w terminalach zdalnych trzeba odznaczyć Terminal > Preferences > Profiles > Advanced > Set locale environment variables at startup


# inne
```
??? brew install imagemagick
brew install mc

```

# Narzędzia i programy
* https://github.com/radgost/handbook/blob/master/narzedzia.md

