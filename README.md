# GFAB - Gestão de Fabricação

Sistema desenvolvido para apoiar o controle do processo de fabricação da Fábrica da Parex Engenharia em Vazante - MG.

O projeto foi construído utilizando **Power Apps**, **Power Automate** e **SharePoint**, com o objetivo de centralizar o acompanhamento dos itens fabricados por projeto, permitindo visualizar o status de fabricação por disciplina e melhorar a rastreabilidade das informações.

---

## Objetivo do Projeto

O **GFAB - Gestão de Fabricação** foi desenvolvido para resolver a ausência de um método digital centralizado para controle da fabricação.

Antes da implantação do sistema, o acompanhamento dos itens dependia de controles manuais, planilhas e comunicação direta entre os responsáveis, dificultando a consulta rápida do status de cada item.

Com o GFAB, a equipe passa a ter uma solução integrada para registrar, consultar e acompanhar o avanço dos projetos e componentes fabricados.

---

## Problema Identificado

A Fábrica da Parex Engenharia precisava de uma forma mais eficiente para acompanhar o processo de fabricação dos itens.

Entre os principais problemas observados estavam:

* Falta de centralização das informações;
* Dificuldade para saber o status atual de cada item;
* Dependência de verificações manuais;
* Baixa rastreabilidade do processo;
* Dificuldade para acompanhar diferentes disciplinas da fabricação;
* Necessidade de padronizar o controle dos projetos.

---

## Solução Desenvolvida

A solução proposta foi a criação de um sistema utilizando a Power Platform, composto por aplicativos, fluxos automatizados e listas do SharePoint.

O sistema permite o controle dos projetos de fabricação, seus respectivos componentes e o avanço de cada item dentro das etapas produtivas.

Entre as disciplinas e etapas acompanhadas pelo sistema, podem estar:

* Engenharia;
* Suprimentos;
* Preparação;
* Montagem;
* Solda;
* Jateamento;
* Pintura;
* Expedição.

---

## Tecnologias Utilizadas

* **Microsoft Power Apps**
* **Microsoft Power Automate**
* **Microsoft SharePoint**
* **Power Fx**
* **Listas do SharePoint**
* **Bibliotecas de documentos do SharePoint**

---

## Estrutura Geral do Projeto

O projeto é composto pelos seguintes arquivos principais:

```text
GFAB Adm.msapp
GFAB Operação.msapp
extrair_projeto.zip
processar_CDP_assincrono.zip
solicitar_processamento_CDP.zip
excluir_fabricacao_completa.zip
```

---

## Aplicativos Power Apps

### GFAB Adm

Aplicativo administrativo utilizado para gerenciar os dados principais do sistema.

De forma geral, este aplicativo é responsável por funções como:

* Cadastro e gerenciamento de projetos;
* Consulta de componentes;
* Acompanhamento dos dados administrativos;
* Integração com listas do SharePoint;
* Acionamento de fluxos do Power Automate;
* Controle geral das informações da fabricação.

### GFAB Operação

Aplicativo voltado para o uso operacional da fábrica.

De forma geral, este aplicativo permite:

* Consultar os projetos em fabricação;
* Visualizar componentes;
* Atualizar status de fabricação;
* Registrar avanço dos itens;
* Apoiar a equipe operacional no acompanhamento diário.

---

## Fluxos Power Automate

O projeto possui fluxos automatizados utilizados para processar informações e manter a integração entre Power Apps e SharePoint.

### solicitar_processamento_CDP

Fluxo responsável por iniciar a solicitação de processamento das informações relacionadas ao CDP.

### processar_CDP_assincrono

Fluxo responsável por processar os dados do CDP de forma assíncrona, permitindo que o sistema trate informações de fabricação sem depender de execução manual direta.

### extrair_projeto

Fluxo responsável por extrair informações de projeto e apoiar o cadastro ou atualização dos dados no sistema.

### excluir_fabricacao_completa

Fluxo responsável por excluir informações completas relacionadas a uma fabricação, quando necessário.

---

## Base de Dados

A base de dados do sistema é estruturada no SharePoint, utilizando listas e bibliotecas para armazenar informações do processo de fabricação.

A estrutura pode conter dados como:

* Projetos;
* Componentes;
* Etapas de fabricação;
* Status dos itens;
* Informações de disciplinas;
* Arquivos relacionados ao projeto;
* Documentos de apoio.

---

## Funcionamento Geral

O funcionamento do sistema pode ser resumido da seguinte forma:

1. O projeto de fabricação é cadastrado no sistema;
2. Os componentes relacionados ao projeto são registrados;
3. Os dados são armazenados em listas do SharePoint;
4. Os fluxos do Power Automate processam informações auxiliares;
5. A equipe acompanha o avanço dos componentes pelo aplicativo;
6. O status dos itens é atualizado conforme a evolução da fabricação;
7. A gestão consegue consultar as informações de forma centralizada.

---

## Benefícios do Sistema

A implantação do GFAB trouxe benefícios para a rotina da fábrica, como:

* Maior controle sobre os itens fabricados;
* Redução de consultas manuais;
* Melhor rastreabilidade das informações;
* Padronização do acompanhamento da fabricação;
* Facilidade para visualizar o status dos projetos;
* Organização das etapas produtivas;
* Integração com o ambiente Microsoft já utilizado pela empresa.

---

## Requisitos para Uso

Para utilizar ou adaptar este projeto, é necessário possuir acesso ao ambiente Microsoft 365 com permissões para:

* Power Apps;
* Power Automate;
* SharePoint;
* Criação e edição de listas;
* Criação e edição de fluxos;
* Importação de aplicativos `.msapp`.

---

## Como Importar os Aplicativos

1. Acesse o Power Apps Studio;
2. Entre no ambiente correto da empresa;
3. Clique em **Aplicativos**;
4. Selecione a opção para importar ou abrir um aplicativo;
5. Carregue o arquivo `.msapp`;
6. Verifique as conexões utilizadas;
7. Ajuste as conexões para o SharePoint e Power Automate;
8. Salve e publique o aplicativo.

---

## Como Importar os Fluxos

1. Acesse o Power Automate;
2. Entre no ambiente correto;
3. Clique em **Meus fluxos**;
4. Selecione a opção de importação;
5. Importe os arquivos `.zip`;
6. Configure as conexões exigidas;
7. Ajuste os caminhos das listas e bibliotecas do SharePoint;
8. Salve e teste cada fluxo.

---

## Observações Importantes

Este projeto foi desenvolvido para atender uma necessidade específica da Fábrica da Parex Engenharia em Vazante - MG.

Caso seja utilizado em outro ambiente, será necessário revisar:

* Nomes das listas do SharePoint;
* Conexões dos aplicativos;
* Conexões dos fluxos;
* Permissões dos usuários;
* Estrutura das bibliotecas;
* Regras de negócio internas;
* Caminhos utilizados nas automações.

---

## Autor

**Felipe Monteiro Reblin**
Curso: Análise e Desenvolvimento de Sistemas

---

## Projeto de Extensão

Este projeto foi desenvolvido como parte das atividades de Projeto de Extensão do curso de Análise e Desenvolvimento de Sistemas, com foco na aplicação prática da tecnologia para solucionar uma necessidade real de uma organização.

---

## Licença

Este repositório possui finalidade acadêmica e demonstrativa.

O uso, adaptação ou distribuição dos arquivos deve respeitar as regras internas da organização envolvida e as permissões aplicáveis ao ambiente Microsoft utilizado.
