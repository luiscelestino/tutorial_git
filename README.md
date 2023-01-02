# Tutorial git

> Status: Em desenvolvimento

## git add
- Coloca arquivo modificado na area stage.
```
git add .
```

## git clone
- Copia um repositorio de origem para a maquina local.
```
git clone <url>
```

- Copia uma branch do repositorio de origem para a maquina local.
```
git clone -branch new_feature <url>
```

## git checkout
- Cria uma nova branch, se ela nao existe, e aponta para ela. Apenas apos o primeiro push sobre esta branch que ela aparecera no repositorio.
```
git checkout -b desenvolvimento
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

- Alteraçoes do projeto muitos detalhes (inclui diff)
```
git log -p
```

- Alteraçoes do projeto sem detalhes
```
git log --online
```

- Alteraçoes do projeto realizadas por um autor especifico
```
git log --author="Luis Celestino"
```

- Alteraçoes do projeto realizadas dentro de um periodo especifico
```
git log --since=2.month.ago --until=1.day.ago
```

- Alteraçoes do projeto formatadas (https://devhints.io/git-log-format)
```
git log --pretty="format:%h %an %ai %s"
```

## git pull
- Copia e exibe alteraçoes do repositorio de origem para a maquina local.
```
git pull <url>
```

## git push
- Envia alteraçoes commitadas para o branch 'main' do repositorio de origem.
```
git push origin main
```

- Envia alteraçoes commitadas para o branch 'desenvolvimnento' do repositorio de origem.
```
git push origin desenvolvimento
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

## git switch
- Modifica a branch atual
```
git switch main
```
```
git switch desenvolvimento
```
