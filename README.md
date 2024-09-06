# fletApps
Some flet Apps examples for MacOs, Linux, Web, Android and iPhone

# Installation of development environment on Linux and MacOs

## Installation on Linux
install VSCode via deb package

(ctrl+shift+p) command palette: digitare 'Python: Create Enviroinment"
viene scaricato il venv python e creato un env python

### Flet Installation 
pip install --upgrade flet

pip install --upgrade pyinstaller

### Install Flutter
follow instruction on website...
install via VSCode cmd palette

## Installazione on Mac

### Installazione XCode
download xcode da appstore
sudo sh -c 'xcode-select -s /Applications/Xcode.app/Contents/Developer && xcodebuild -runFirstLaunch'
sudo xcodebuild -license

### Install di Flutter
brew install --cask flutter

sudo gem install cocoapods (dopo aver già installato ruby gems con asciidoctor-epub (vedi documento github))

### install IPhone Simulator
xcodebuild -downloadPlatform iOS
open -a Simulator

### install Android studio
brew install --cask android-studio

### Installazione di Python
brew install python@3.12

### installazione virtualenv
brew install virtualenv

### install VsCode
brew install --cask visual-studio-code

run code .

install Python plugin

install Error Lens Plugin

### install Flet

create .venv da command palette: "python: create enviroinment" in command palette

open VSCode Terminal

python3 -m venv .venv
source .venv/bin/activate

pip install flet --upgrade

flet create --project-name myCounter --description 'My Counter App' --template counter myCounter

flet run myCounter

flet run --ios (da verificare come mai non apre su ios/android forse firewall)

<flet_app_directory>% flet build <target_platform>

con where <target_platform> could be one of the following: apk, aab, ipa, web, macos, windows, linux.

flet build macos

flet pack counter.py

flet build apk --project count  (con file main.py)

flet build apk --project count  --module counter.py (forse!)

## Upgrade

### on Linux

sudo apt update

sudo apt dist-upgrade

'check update of Android Studio application'

'.../bin/studio.sh  check update of Android SDK Manager'

cd .../Develop/Python/fletApps

flutter upgrade

flutter doctor -v

code .

'Open VsCode Terminal'

source .venv/bin/activate

### on Mac

'check update of xCode on App Store!'

'check update of Android Studio application'

'check update of Android SDK Manager'

brew update

brew upgrade

brew upgrade --cask flutter

sudo gem update
or
sudo gem update cocoapos
or
sudo gem install cocoapods (dopo aver già upgradato ruby gems con brew upgrade)

flutter doctorv -v

code .

'Open VsCode Terminal'

source .venv/bin/activate

pip install --upgrade pip

pip install --upgrade flet

pip install --upgrade PyInstaller

## Develop

### on Linux
or
### on Mac

open Terminal

cd Develop\Python\fletApps

code .

source .venv/bin/activate

flet create --project-name myCounter --description 'My Counter App' --template counter myCounter

flet run myCounter

flet run --ios counter.py (da verificare come mai non apre su ios/android forse firewall)
flet run --android counter.py
flet run --web counter.py
flet run counter.py (app linux/mac/windows)

<flet_app_directory>% flet build <target_platform>

where <target_platform> could be one of the following: apk, aab, ipa, web, macos, windows, linux.

flet build macos

flet pack counter.py

flet build apk --project count  (con file main.py)

flet build apk --project count  --module counter.py 

flet build web
poi dalla dir del file index.html lanciare
python3 -m http.server
aprire il browser su http://localhost:8000/ per lanciare l'app web

oppure flet run --web
