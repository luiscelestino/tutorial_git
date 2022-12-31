# Tutorial git

> Status: Em desenvolvimento

## git add
- Coloca arquivo modificado na area stage.
```
git add *
```

## git clone
- Copia um repositorio de origem para a maquina local.
```
git clone <url>
```

## git commit
- Commita arquivos da area de stage.
```
git commit . -m "mensagem"
```

- Commita arquivos, adicionando automaticamente na area de stage.
```
git commit . -a -m "mensagem"
```

## git log
- Alteraçoes do projeto com detalhes
```
git log
```

- Alteraçoes do projeto sem detalhes
```
git log --online
```

## git pull
- Copia e exibe alteraçoes do repositorio de origem para a maquina local.
```
git pull <url>
```

## git push
- Envia alteraçoes commitadas para o branch main do repositorio de origem.
```
git push origin main
```

## git restore
- Volta versao do codigo local para um commit anterior.
```
git restore --source a01bgd2 .
```

- Volta versao de um arquivo local para um commit anterior.
```
git restore --source a01bgd2 arquivo.txt
```

- Volta versao do codigo do repositorio para um commit anterior.
```
git restore --source a01bgd2 .
git commit -a -m "mensagem"
git push origin main
```

## git status
- Verifica modificaçoes locais.
```
git status
```
