# ConstruindoUmEsquemaConceitualParaBancoDeDados
Objetivo:
Cria o esquema conceitual para o contexto de oficina com base na narrativa fornecida

Narrativa:
Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica
Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas
Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.
A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços
A mesma equipe avalia e executa os serviços
Os mecânicos possuem código, nome, endereço e especialidade
Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.

# Sistema de Controle de Ordens de Serviço - Oficina Mecânica

Este repositório contém o esquema conceitual para o controle e gerenciamento de ordens de serviço em uma oficina mecânica. O sistema permite que os clientes levem seus veículos para conserto ou revisão periódica. Cada veículo é registrado com uma ordem de serviço, que detalha os serviços a serem realizados e os custos associados.

## Entidades e Relacionamentos

As principais entidades do sistema incluem:

- **Cliente**: Representa o cliente que solicita serviços na oficina.
- **Veículo**: Representa o veículo do cliente que será consertado ou revisado.
- **Ordem de Serviço (OS)**: Contém informações sobre os serviços a serem realizados em um veículo.
- **Mecânico**: Profissional responsável pela execução dos serviços.
- **Equipe**: Grupo de mecânicos que trabalham em uma ordem de serviço.
- **Serviço**: Representa um tipo específico de serviço executado no veículo.
- **Tabela de Referência de Mão de Obra**: Define o custo de mão de obra baseado no tempo estimado para cada serviço.
- **Peça**: Refere-se às peças usadas na execução dos serviços.

### Relacionamentos

- Um **Cliente** pode ter vários **Veículos**.
- Um **Veículo** pode ter várias **Ordens de Serviço**.
- Uma **Ordem de Serviço** pode ter vários **Serviços** e **Peças**.
- Cada **Ordem de Serviço** está associada a um **Cliente** e a um **Veículo**.
- Um **Mecânico** pertence a uma **Equipe** que executa os serviços nas **Ordens de Serviço**.

## Licença

Este projeto está licenciado sob a MIT License.
