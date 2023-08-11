# LAMP (Apache2, MySQL und PHP8.2)

* Für eine Automatische Installation, so führe diesen Script/Command aus:

```bash
Coming Soon
```



* Manuelle Installation

```bash
while true
do
  Dein_Java_File/java -jar spigot.jar
  echo 'Willst Du den Server komplett stoppen, drücke STRG+C!'
  echo "Neustart in:"
  for i in 5 4 3 2 1
  do
  echo "$i..."
  sleep 1
  done
  echo 'Server neustart!'
done
```

* Ein Beispiel für einen Pfad

```bash
/usr/lib/jvm/adoptopenjdk-8-hotspot-amd64/bin/java -jar spigot.jar
```

* Nun gebe deiner Startdatei Rechte zum Ausführen

```bash
chmod +x start.sh
```

* Nun kannst du dein Server starten:

```bash
./start.sh
```

* Falls du dein Server im Hintergrund laufen lassen möchtest:

```bash
screen -AmdS Session_Name ./start.sh
```
