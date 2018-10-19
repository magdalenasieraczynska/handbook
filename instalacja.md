
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

* instalacja Pow http://pow.cx/

```
brew install pow

# Create the required host directories:
mkdir -p ~/Library/Application\ Support/Pow/Hosts
ln -s ~/Library/Application\ Support/Pow/Hosts ~/.pow

# Setup port 80 forwarding and launchd agents:
sudo pow --install-system
pow --install-local

# fix do pow.cx (aby pokazywał poprawnie błędy w aplikacji zamiast "End of file reached"):

curl -L https://gist.githubusercontent.com/RobinDaugherty/2731f20d303e6506d451384df2189210/raw/b52e6231170b3dce39633db29634dc892751910f/pow_better_errors_fix.patch | patch ~/Library/Application\ Support/Pow/Versions/0.6.0/node_modules/nack/lib/nack/server.rb

```
projekty

```
cd
mkdir projects
mkkir projects/radgost
cd ~/.pow; ln -s ~/projects/radgost

```
teraz można odpalić:
http://radgost.test


* PostgreSQL
```
brew install postgresql@9.5
```
* MySQL

```
brew install mysql@5.6

#wstawic do ~/.bash_profile aby dzialalo polecenie mysql:
echo 'export PATH="/usr/local/opt/mysql@5.6/bin:$PATH"' >> ~/.bash_profile

brew services start mysql@5.6

cp /usr/local/Cellar/mysql\@5.6/5.6.36_1/support-files/my-default.cnf /usr/local/etc/my.cnf 

echo 'max_allowed_packet=64M' >> /usr/local/etc/my.cnf


```

percona
```
brew install percona-toolkit
```

* inne
```
brew install imagemagick
brew install Caskroom/cask/wkhtmltopdf 
brew install mc

```

* Narzędzia i programiy
https://github.com/radgost/handbook#narz%C4%99dzia--programy

