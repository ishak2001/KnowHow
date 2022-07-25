# Nginx Installation

* Aktualisiere die Paketlisten & installiere die Updates.

```bash
apt update && apt upgrade -y
```

* Installiere nun Nginx

```bash
apt install nginx -y
```

* Dein Verzeichnis für dein Web Server findest du unter ```/var/www/html```
* Erreichen tust du dein Web Server indem du im Browser deine ```IP``` oder deine ```Domain``` eingibst, die du mit einem A Record versehen werden muss.
