# Como instalar o Google Chrome

Baixe a chave do repositório e depois adicione ela ao sistema:
```bash
$ wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
```

Depois de adicionado a chave, adicione o repositório ao sistema:
```bash
$ sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
```

Depois de adicionado o repositorio, é necessario atualizar as referências do sistema:
```bash
$ sudo apt-get update
```

Agora é só instalar o Chrome:
```bash
$ sudo apt-get install google-chrome-stable
```

-----

[Voltar](README.md)

