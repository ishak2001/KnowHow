## Python 3.11 Installation

* Aktualisiere die Paketlisten & installiere die Updates.
```bash
apt update && apt upgrade -y
```

* Installieren Sie die benötigten Pakete
``` bash
apt install wget build-essential libncursesw5-dev libssl-dev \
     libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev libffi-dev zlib1g-dev   -y
```

* Python3.11 Installieren
``` bash
wget https://www.python.org/ftp/python/3.11.3/Python-3.11.3.tgz
```

* Python3.11 Extrahieren
``` bash
tar xzf Python-3.11.3.tgz 
```

* Für die Kompilierung von Python3.11 
``` bash
./configure --enable-optimizations 
```

* Um Python3.11 ui Installieren
``` bash
make altinstall
```

Python3.11 Ist erfolgreich Installiert
