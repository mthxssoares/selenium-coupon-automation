# Selenium Web Automation

![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge\&logo=selenium\&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge\&logo=openjdk\&logoColor=white)
![Cucumber](https://img.shields.io/badge/Cucumber-23D96C?style=for-the-badge\&logo=cucumber\&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit-25A162?style=for-the-badge\&logo=junit5\&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge\&logo=apachemaven\&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge\&logo=github-actions\&logoColor=white)

Projeto de automação de testes web com foco principal em **Selenium WebDriver**, utilizando **Java**, **Cucumber**, **JUnit** e **Maven** para validar o fluxo de geração de cupom de desconto no site da **QAzando**.

Este projeto representa meu primeiro contato prático com automação web usando Selenium, aplicando boas práticas como escrita de cenários em Gherkin, organização com Page Object, geração de relatórios e preparação para execução em fluxo de **CI/CD** com **GitHub Actions**.

---

## Objetivo do projeto

O objetivo deste projeto é praticar e demonstrar conhecimentos em **automação de testes web com Selenium WebDriver**, utilizando o Selenium como principal ferramenta para interação com elementos da página e validação do comportamento da aplicação.

Além disso, o projeto também aplica boas práticas de organização e execução de testes automatizados, como:

* Escrita de cenários em **Gherkin**;
* Organização dos testes com **Cucumber**;
* Execução dos testes com **JUnit**;
* Gerenciamento de dependências com **Maven**;
* Estruturação inicial com padrão **Page Object**;
* Geração de relatórios de execução;
* Preparação para integração contínua com **GitHub Actions**.

---

## Tecnologias utilizadas

* Selenium WebDriver
* Java
* Maven
* Cucumber
* JUnit 4
* Gherkin
* ChromeDriver
* Git
* GitHub
* GitHub Actions
* Cluecumber Report

---

## Funcionalidade automatizada

O projeto automatiza um fluxo web no site da **QAzando**, validando a geração de um cupom de desconto.

Fluxo principal:

1. Acessar o site da QAzando;
2. Informar um e-mail;
3. Clicar no botão para gerar o cupom;
4. Validar se o código do cupom foi exibido corretamente.

---

## Cenário de teste

Exemplo de cenário escrito em Gherkin:

```gherkin
#language: pt

Funcionalidade: Gerar cupom de desconto

  @gerar-cupom
  Cenário: Gerar cupom de desconto com sucesso
    Dado que acesso o site da QAzando
    Quando informo meu e-mail
    E clico no botão de ganhar cupom
    Então devo visualizar o código do cupom de desconto

```
## Sobre os diretórios

### `features`

Contém os cenários de teste escritos em linguagem **Gherkin**.

### `steps`

Contém a implementação dos passos descritos nos arquivos `.feature`.

### `pages`

Contém as classes responsáveis por representar as páginas do sistema, seguindo a ideia do padrão **Page Object**.

### `runner`

Contém a classe responsável por executar os testes automatizados com **Cucumber** e **JUnit**.

---

## Pré-requisitos

Antes de executar o projeto, é necessário ter instalado:

* Java configurado na máquina;
* Maven configurado no PATH;
* Google Chrome instalado;
* Git instalado;
* IDE de sua preferência, como IntelliJ IDEA ou VS Code.

---

## Como executar o projeto

Após baixar ou clonar o repositório, acesse a pasta raiz do projeto, onde está localizado o arquivo `pom.xml`.

Caso tenha baixado o projeto em formato `.zip`, extraia o arquivo e abra a pasta do projeto na sua IDE, como IntelliJ IDEA ou VS Code.

A estrutura principal deve conter:

```text
src/
pom.xml
README.md

---

## Executando testes por tag

O projeto utiliza tags do Cucumber para organizar a execução dos testes.

Exemplo de tag utilizada:

```text
@gerar-cupom
```

Para executar testes por tag, use:

```bash
mvn test -Dcucumber.filter.tags="@gerar-cupom"
```

---

## Integração Contínua com GitHub Actions

Este projeto possui uma estrutura preparada para execução automática dos testes utilizando **GitHub Actions**.

A ideia do CI é permitir que os testes sejam executados automaticamente a cada alteração enviada para o repositório, ajudando a garantir maior confiabilidade no código.

Fluxo esperado:

* O código é enviado para o GitHub;
* O GitHub Actions inicia automaticamente;
* O ambiente é configurado;
* Os testes são executados com Maven;
* Os relatórios são publicados como artefato da execução.

---


## Boas práticas aplicadas

* Uso do Selenium WebDriver como ferramenta principal de automação web;
* Separação entre cenários, steps e pages;
* Escrita de testes em Gherkin;
* Uso de tags para organizar a execução;
* Geração de evidências por relatório;
* Estrutura preparada para CI;
* Uso do Maven para gerenciamento de dependências;
* Organização inicial baseada no padrão Page Object.

---

## Aprendizados com o projeto

Com este projeto, foi possível praticar conceitos importantes de QA e automação, como:

* Criação de cenários de teste automatizados;
* Automação de interações web com Selenium WebDriver;
* Localização e manipulação de elementos em páginas web;
* Escrita de testes com Cucumber;
* Execução de testes via Maven;
* Configuração de runner com JUnit;
* Geração de relatórios de testes;
* Primeiros passos com CI usando GitHub Actions.

---

## Status do projeto

Projeto em desenvolvimento e evolução contínua.

Próximas melhorias possíveis:

* Adicionar mais cenários de teste;
* Melhorar a organização das classes Page Object;
* Implementar screenshots em caso de falha;
* Adicionar execução em modo headless;
* Melhorar os relatórios gerados;
* Expandir a cobertura dos testes automatizados.

---

## Autora

**Matheus Soares**

QA Enthusiast | Software Testing | Testes Web, Desktop e Mobile | IA & Chatbots | 
