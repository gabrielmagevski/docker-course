## Commands

#### docker container ls

listar os containers

#### docker container run -ti hello-world

se a image "hello-world" não existir no host, o docker client faz o pull para daemon e imprimi a image

nisso o docker daemon criou um container novo em cima da image que pedimos acima

#### docker container ls -a

vai mostrar os que estão em execução e os que não estão mais

### docker container run -ti

#### -ti

O menos _-ti_ faz com que já entramos dentro do container assim que ele for criado.

_O que eu quero quero que o -ti faça?_

Execute o container mas para ele eu quero ter um terminal e interatividade

#### ps -ef

Mostra os processos em execução

#### cat /etc/issue

Mostra a versão e o linux usado

### exit

Sair do container _matando o processo_

#### OU CTRL + D

Se executarmos o _CTRL + D_ ou _exit_ dentro do container a gente mata ele

#### Sair do container sem mata-lo

_CTRL + P + Q_

### docker container attach <Nome do container> ou <ID HASH>

Vamos conectar no container já em execução

#### cat /etc/redhat-release

Comando para vermos se estamos dentro do container mesmo.

## Conceitos

#### Entrypoint

todo container o possue, o que ele é? é o principal processo do container, se ele não estiver vivo o container morre
