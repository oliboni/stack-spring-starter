## STACKSPOT
**Padronização e compartilhamento de Stacks para ganhar velocidade e escalar o desenvolvimento com confiança**

## *Criar conta*
> Criar uma conta e fazer download do CLI no site oficial <https://stackspot.com/pt>

> Após o download no terminal rodar:
> ``stk login``

## Stack

### Criar app com stack default (básica)
```
stk create app test-stackfile -S stack-spring-starter/default
```
### Criar app com stack web com a aplicação dos plguins:
```
stk create app test-stackfile2 -S stack-spring-starter/template-plugin-db
```

## Plugins

Existem dois plugins, um para adicionar as configs do database e outro para adicionar as configs do flyway

### Database
```
stk apply plugin -p /Users/<USER>/<PATH>/stack-spring-starter/db-config-plugin
```

### Flyway
```
stk apply plugin -p /Users/<USER>/<PATH>/stack-spring-starter/flyway-plugin
```

## Comandos úteis:


| Função               | Comando                                 |
|----------------------|-----------------------------------------|
| Criar nova stack     | stk create stack *<NOME_STACK>*         |
| Criar nova stackfile | stk create stackfile *<NOME_STACKFILE>* |
| Criar novo plugin    | stk create plugin *<NOME_PLUGIN>*       | 
| Listar stacks        | stk list stack                          | 
| Listar stacksfile`s  | stk list stackfile                      |
| Listar Plugins       | stk list plugin                         |
