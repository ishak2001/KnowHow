# Portainer Installation

{% hint style="warning" %}
für die Installation ist Docker nötig. Falls du diese nicht installiert hast, kannst du dies hier ganz schnell nachholen -> [Docker Installation](docker-installation.md)
{% endhint %}

* Aktualisiere die Paketlisten & installiere die Updates.

```bash
apt update && apt upgrade -y
```

* Erstelle ein Verzeichnis für `Portainer`

```bash
mkdir ~/portainer
```

* Navigiere ins Verzeichnis

```bash
cd ~/portainer
```

* Erstelle nun eine Compose Datei

```bash
nano docker-compose.yml
```

* Füge nun diesen Code ein

```bash
version: "3.3"
services:
    portainer:
      image: portainer/portainer-ce:latest
      container_name: portainer
      restart: always
      privileged: true
      volumes:
        - ./data:/data:Z
        - /var/run/docker.sock:/var/run/docker.sock:Z
      ports:
        - 9443:9443
```

* Bringe dein `Portainer` zum laufen

```bash
docker-compose up -d
```

* Die Website kannst du unter `https://<DeineServerIP>:9443` erreichen.
