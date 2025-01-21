# Desafio: Sistema de Controle e Gerenciamento de Oficina Mecânica

## Descrição do Desafio

Este repositório contém o esquema conceitual desenvolvido para o **controle e gerenciamento de ordens de serviço (OS)** em uma oficina mecânica. O objetivo principal foi modelar um sistema que gerencia a execução de ordens de serviço em uma oficina, desde o cadastro do cliente até a finalização e cobrança dos serviços realizados.

A narrativa fornecida descreve um fluxo de trabalho envolvendo **clientes**, **veículos**, **mecânicos** e **ordens de serviço**, onde os mecânicos executam serviços de manutenção ou revisão, com base em uma tabela de referência de mão-de-obra e peças. O modelo foi construído para representar adequadamente essas entidades e seus relacionamentos, garantindo que todos os aspectos do processo sejam considerados.

## Objetivo

O objetivo deste desafio foi criar um **esquema conceitual** para o contexto de uma oficina mecânica, levando em conta os seguintes pontos-chave:

1. **Clientes**: Os clientes trazem seus veículos para consertos ou revisões periódicas.
   
2. **Veículos**: Cada veículo é designado a uma equipe de mecânicos, que irá identificar e executar os serviços necessários.

3. **Ordens de Serviço (OS)**: As ordens de serviço contêm informações sobre os serviços a serem executados, a equipe responsável, o valor dos serviços e das peças, a data de emissão e a data de conclusão dos trabalhos.

4. **Mecânicos**: Cada mecânico possui informações como código, nome, endereço e especialidade.

5. **Tabela de Referência de Mão-de-Obra**: Utilizada para calcular o valor de cada serviço executado na oficina.

## Estrutura do Diagrama

O modelo conceitual foi representado por meio de um **diagrama Entidade-Relacionamento (ER)**, onde são descritas as principais entidades envolvidas no processo da oficina mecânica, como **Cliente**, **Veículo**, **Mecânico**, **Ordem de Serviço (OS)** e **Tabela de Referência de Mão-de-Obra**. As entidades foram detalhadas com seus respectivos atributos e relacionamentos, conforme a narrativa fornecida.

### Entidades e Atributos:

- **Cliente**: Representa o cliente da oficina, com atributos como nome, CPF/CNPJ e endereço.
  
- **Veículo**: Representa os veículos dos clientes, com atributos como modelo, ano e placa.

- **Mecânico**: Representa os mecânicos da oficina, com atributos como código, nome, endereço e especialidade.

- **Ordem de Serviço (OS)**: Contém informações como número, data de emissão, status, data de conclusão e o valor total dos serviços e peças.

- **Tabela de Referência de Mão-de-Obra**: Utilizada para calcular o valor dos serviços com base no tipo de serviço executado.

- **Serviço**: Representa os serviços a serem realizados, com atributos como tipo e valor calculado.


### Relacionamentos:

- **Cliente → Veículo**: Um cliente pode ter múltiplos veículos.
  
- **Veículo → Ordem de Serviço (OS)**: Um veículo pode ter múltiplas ordens de serviço associadas.

- **Ordem de Serviço (OS) → Mecânico**: A OS é atribuída a uma equipe de mecânicos para execução.

- **Ordem de Serviço (OS) → Serviço**: A OS inclui múltiplos serviços a serem executados.


## Tecnologias e Ferramentas Utilizadas

- **GitHub**: Para versionamento de código e documentação do projeto.
- **Ferramenta de Modelagem ER**: Para criar e ajustar o diagrama de Entidade-Relacionamento (ER).
- **Ferramentas de Banco de Dados**: Modelagem de banco de dados relacional (não incluído diretamente aqui, mas o modelo pode ser implementado em SQL ou outra tecnologia de banco de dados).

## Conclusão

Este desafio foi uma excelente oportunidade para aplicar e aprimorar minhas habilidades em **modelagem de dados** e compreender os aspectos essenciais de um **sistema de gerenciamento de ordens de serviço** em uma oficina mecânica. Através da construção do modelo conceitual, pude integrar diferentes entidades e processos envolvidos na operação de uma oficina, criando uma solução escalável e de fácil implementação para esse tipo de negócio.

Este projeto agora está disponível no GitHub, permitindo que outras pessoas possam verificar, colaborar e adaptar o modelo para suas necessidades específicas.
