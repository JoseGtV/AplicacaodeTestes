# Projeto JAVA Qualidade de Software
Este é um projeto Java simples que demonstra um CRUD simples

## Pré-requisitos

Antes de começar, verifique se você atende aos seguintes requisitos:
- Java Development Kit (JDK) instalado na sua máquina
- Apache Maven (opcional, se estiver usando o Maven para gerenciar o projeto)

### Alunos
 - José Gustavo da Silva Oliveira - RA:223126
 - Matheus Henrique Correa Macarenhas - RA:200044
 - João Vitor Candini - RA: 212032
 
## BDD

Feature: Funcionalidades do Menu Inicial

  Scenario: Clicar no botão "OK" do menu inicial sem digitar nenhum valor
    Given que estou no menu inicial
    When eu clico no botão "OK"
    Then uma mensagem é exibida solicitando o preenchimento do campo

  Scenario: Clicar no botão "Cancel" do menu inicial sem nenhum valor digitado
    Given que estou no menu inicial
    When eu clico no botão "Cancel"
    Then nada acontece

  Scenario: Clicar no botão "Cancel" do menu inicial com um valor digitado
    Given que estou no menu inicial e um valor está digitado
    When eu clico no botão "Cancel"
    Then o valor digitado é apagado

  Scenario: Clicar no botão de fechar "x" do menu inicial
    Given que estou no menu inicial
    When eu clico no botão de fechar "x"
    Then a aplicação é fechada

  Scenario: Sair do menu inicial
    Given que estou no menu inicial
    When eu digito "9" no campo de texto e clico no botão "OK"
    Then a aplicação é fechada

Feature: Funcionalidades do Menu de Entrada de Atletas

  Scenario: Abrir tela de "Entrada de Atletas"
    Given que estou no menu inicial
    When eu digito "1" no campo de texto e clico no botão "OK"
    Then a tela de "Entrada de Atletas" é aberta

  Scenario: Clicar no botão "OK" do menu de Entrada de Atletas sem digitar nenhum valor
    Given que estou no menu de Entrada de Atletas
    When eu clico no botão "OK"
    Then uma mensagem é exibida solicitando o preenchimento do campo

  Scenario: Clicar no botão "Cancel" do menu de Entrada de Atletas sem nenhum valor digitado
    Given que estou no menu de Entrada de Atletas
    When eu clico no botão "Cancel"
    Then nada acontece

  Scenario: Clicar no botão "Cancel" do menu de Entrada de Atletas com um valor digitado
    Given que estou no menu de Entrada de Atletas e um valor está digitado
    When eu clico no botão "Cancel"
    Then o valor digitado é apagado

  Scenario: Clicar no botão de fechar "x" do menu de Entrada de Atletas
    Given que estou no menu de Entrada de Atletas
    When eu clico no botão de fechar "x"
    Then volto para o Menu Inicial

  Scenario: Abrir tela de "Nome do Corredor"
    Given que estou no menu de Entrada de Atletas
    When eu digito "1" no campo de texto e clico no botão "OK"
    Then a tela de "Nome do Corredor" é aberta

  Scenario: Clicar no botão "OK" do menu de Entrada de Corredores sem digitar nenhum valor
    Given que estou na tela de "Nome do Corredor"
    When eu clico no botão "OK"
    Then uma mensagem é exibida solicitando o preenchimento do campo

  Scenario: Clicar no botão "Cancel" do menu de Entrada de Corredores sem nenhum valor digitado
    Given que estou na tela de "Nome do Corredor"
    When eu clico no botão "Cancel"
    Then nada acontece

  Scenario: Clicar no botão "Cancel" do menu de Entrada de Corredores com um valor digitado
    Given que estou na tela de "Nome do Corredor" e um valor está digitado
    When eu clico no botão "Cancel"
    Then o valor digitado é apagado

  Scenario: Clicar no botão de fechar "x" do menu de Entrada de Corredores
    Given que estou na tela de "Nome do Corredor"
    When eu clico no botão de fechar "x"
    Then volto para o Menu de Entrada de Atletas

  Scenario: Preencher nome do corredor com números
    Given que estou na tela de "Nome do Corredor"
    When eu preencho o campo de nome do corredor com números
    Then uma mensagem informando que o nome está incorreto é exibida

  Scenario: Preencher corretamente o nome do corredor
    Given que estou na tela de "Nome do Corredor"
    When eu preencho corretamente o campo de nome do corredor e clico em "OK"
    Then a tela de preenchimento do número do corredor é aberta

  Scenario: Preencher número do corredor com letras
    Given que estou na tela de preenchimento do número do corredor
    When eu preencho o campo de número do corredor com letras
    Then uma mensagem informando que o número está incorreto é exibida

  Scenario: Preencher corretamente o número do corredor
    Given que estou na tela de preenchimento do número do corredor
    When eu preencho corretamente o campo de número do corredor e clico em "OK"
    Then a tela de preenchimento da velocidade do corredor é aberta

  Scenario: Preencher velocidade do corredor com letras
    Given que estou na tela de preenchimento da velocidade do corredor
    When eu preencho o campo de velocidade do corredor com letras
    Then uma mensagem informando que a velocidade está incorreta é exibida

  Scenario: Preencher corretamente a velocidade do corredor
    Given que estou na tela de preenchimento da velocidade do corredor
    When eu preencho corretamente o campo de velocidade do corredor e clico em "OK"
    Then uma mensagem informando que o registro foi concluído com sucesso é exibida, e volto para tela de menu inicial



