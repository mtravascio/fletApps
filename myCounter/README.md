# A myCounter Flet app

the first counter app.

## To run the app:
```
flet run myCounter
```

## To Build myCounter Web App:
```
flet build web myCounter

flet run --web myCounter
```
or
```
python3 -m http.server nella directory di index.html
```
open the browser su http://localhost:8000/ per lanciare l'app web

## To Build Mac Os App
```
flet build macos myCounter
```
launch ./myCounter/build/macos/mycounter.app

## To Build Linux App
```
flet build linux myCounter
```
launch ./myCounter/build/linux/mycounter

...after that to pack mycounter app (using pyinstaller)
```
flet pack myCounter/main.py
```
launch ./dist/main

## To Build iOS App
```
flet build ipa myCounter
```
To launch...(to be done)

## To Build Android App/Bundle
```
flet build apk myCounter

flet build aab myCounter
```
To launch...(to be done)

