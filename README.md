# Utvecklingsmiljö

I denna mapp finns en Vagrantfile. Den hjälper oss att skapa en virtuell maskin så vi alla har tillgång till samma verktyg så som språk och databaser. För att kunna använda detta måste du [installera Vagrant](https://www.vagrantup.com/intro/getting-started/install.html). 

För att starta den virtuella maskinen skriver du bara
```sh
#!/bin/zsh
vagrant up
```

Sedan kan du logga in i den virtuella maskinen genom att skriva
```sh
#!/bin/zsh
vagrant ssh
```

Efter detta har du tillgång till Lunicores utvecklingsmiljö. Denna mapp är mountad `/vagrant` i den virtuella maskinen.

För att använda jupyter i webläsaren på din lokala dator (guest) skriver du
````sh
#!/bin/zsh
jupyter notebook --ip=0.0.0.0
```
Det är då möjligt att öppna din notebook i webbläsaren genom att skriva
````sh
http://0.0.0.0:8888/tree
```
