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
