# SunnyTravel
## Starten des Frontends
+ gehen Sie in Ordner frontend und öffnen sie die Datei index.html
## Datenbank vorbereiten
+ öffnen Sie ein Terminal im db Verzeichnis
+ docker build -t <dockerhubid>/db_travel .
+ docker run --name postgres -p 5430:5432 -e POSTGRES_PASSWORD=123456 -d <dockerhubname>/db_travel

## Starten des Backends
+ öffnen Sie ein Terminal in dem Ordner backend
  + führen Sie dort npm install aus
+ überprüfen Sie die config.js Datei, ob Port 5430 und Passwort 123456 gesetzt sind
+ starten sie das Backend mit node index.js
