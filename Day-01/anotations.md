## O que é um container no Docker?

Container não é uma máquina virtual.

O container é a forma de fazermos isolamentos, e dentro desses isolamentos existem.

- Processos isolados
- Usuários isolados
- Redes isoladas

...

## Conseguimos isolar os recursos do nosso hardware para algum container?

Sim, conseguimos isolar os recursos para o container como:

- Memória
- CPU
- Disco
- Redes

## Quem são os responsaveis por fazerem esses isolamentos?

### Isolamento lógico

- Que são processos, usuários e etc...

O tipo de isolamento dele é _Namespaces_.

### Isolamento fisíco

- Que são CPUS, Memórias, Disco e Redes

O tipo de isolamento dele é \* _Cgroups_.

## Docker, o que é?

Docker é responsável por gerenciar vários processos, ou serviços, de maneira isolada do host, como banco de dados e uma aplicação, por exemplo, sendo executados em containers diferentes.

## Como funciona a imagem de um container? _importante_

Quando possuímos a imagem de um container, nós temos várias camadas nessa imagem.

Se precisarmos escrever um caracter em uma camada, porém ela é RO. O Docker vai copiar a antiga camada e criarar uma nova camada baseada na antiga para escrevermos.

_Observações:_ Quando temos várias camadas apenas a última camada é possível escrever. O resto é tudo readonly (R.O)

## Container utiliza várias imagens diferentes para cada container?

Não, por que é RO os containers antigos e por isso utiliza a mesma imagem das camadas antigas.

_Obs:_ Caso queira instalar mais coisas no seu container é necessário 1 run com && comercial para instalar tudo 1x só para não termos camadas diferentes e impossibilitando você interagir com a camada anterior.
