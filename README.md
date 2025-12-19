# Oficina Mecânica – Esquema Conceitual de Banco de Dados

Este projeto apresenta a modelagem conceitual de um banco de dados para um sistema de controle e gerenciamento de ordens de serviço (OS) em uma oficina mecânica.

## Contexto
Clientes levam seus veículos à oficina para consertos ou revisões periódicas. Cada veículo é designado a uma equipe de mecânicos, que avalia os serviços necessários, registra uma ordem de serviço e executa os trabalhos após autorização do cliente.

## Principais Regras de Negócio
- Um cliente pode possuir um ou mais veículos.
- Cada ordem de serviço está associada a um único veículo e a uma única equipe.
- A mesma equipe é responsável pela avaliação e execução dos serviços.
- Uma ordem de serviço pode conter vários serviços e várias peças.
- O valor total da OS é composto pela soma dos serviços (mão de obra) e das peças utilizadas.
- Os valores dos serviços são calculados com base em uma tabela de referência de mão de obra.
- A execução dos serviços depende da autorização do cliente.

## Observações
Algumas decisões de modelagem foram tomadas com base na interpretação do contexto, como a criação de entidades associativas para serviços e peças, visando garantir flexibilidade e normalização do modelo.

## Tecnologias
- Modelagem Conceitual (DER)
- Banco de Dados Relacional
