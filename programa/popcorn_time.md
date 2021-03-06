# Como instalar o _Popcorn Time_

![Popcorn Time logo](img/pctlogo.png)

Criar diretório para o _Popcorn Time_:
```bash
$ sudo mkdir /opt/popcorn-time
```

Baixar o fonte:

> Para **32 bits**
```bash
$ sudo wget -qO- https://get.popcorntime.sh/build/Popcorn-Time-0.3.10-Linux-32.tar.xz | sudo tar Jx -C /opt/popcorn-time
```

ou 

> Para **64 bits**
```bash
$ sudo wget -qO- https://get.popcorntime.sh/build/Popcorn-Time-0.3.10-Linux-64.tar.xz | sudo tar Jx -C /opt/popcorn-time
```

Criar um link para o _Popcorn Time_:
```bash
$ sudo ln -sf /opt/popcorn-time/Popcorn-Time /usr/bin/popcorn-time
```

Para criar um _Desktop Launcher_:
```bash
$ sudo gedit /usr/share/applications/popcorntime.desktop
```

Com o arquivo aberto inclua as seguintes propriedades:
```properties
[Desktop Entry]
Version = 1.0
Type = Application
Terminal = false
Name = Popcorn Time
Exec = /usr/bin/popcorn-time
Icon = /opt/popcorn-time/popcorntime.png
Categories = Application;
```

Após salvar o arquivo, inclua um ícone a aplicação:
```bash
$ sudo wget -q -O /opt/popcorn-time/popcorntime.png https://upload.wikimedia.org/wikipedia/commons/6/6c/Popcorn_Time_logo.png
```

Para executar pela linha de comando use o seguinte comando:
```bash
$ popcorn-time
```

Procure o `Popcorn Time` no menu de aplicações e execute-o, para testar.

-----

[Voltar](README.md)