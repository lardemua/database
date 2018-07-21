# Database

*Package* responsável escrita de informação na base de dados Postgresql localizada no servidor do LAR- DEM- UA.  

## Requisitos

 Internet

 Servidor do LAR operacional (ligado à rede).


## Utilização

```
<?xml version="1.0"?>
<launch>
    <node pkg="database" name="database_node" type="database_node"  />
    <param name="dbname" value="atlas_monitoring"  />
    <param name="user" value="*****"  />
    <param name="password" value="*******"  />
    <param name="hostaddr" value="193.137.*******"  />  
    <param name="port" value="5432"  />  
</launch>
```

```
roslaunch database database.launch
```

ATENÇÃO:

Ao terminar os processos, tenha o cuidado de verificar que este processo efetivamente terminou. Caso contrário a página *web* ficaria com informação desatualizada.


## Expansão da base de dados

É aconselhável a criação de mais tabelas adequadas ao tipo de informação, nelas inscrito.

ATENÇÃO:  

Para que a informação deseja disponibilizada na página *web*  [ATLASCAR Live]( http://lars.mec.ua.pt/atlascar_live.html) é necessário adaptar os ficheiros php, javascript, html responsáveis pelo fluxo de informação até à base de dados. Estes ficheiros encontram se no diretório *var/www/*  do servidor do LAR.

Para mais informações consultar os trabalhos de José Viana e/ou Pedro Bouça Nova.

# Instalação

Através do github ATLASCAR.


## Autor

* **Pedro Bouça Nova** - *Dissertação de Mestrado - 2018* -




