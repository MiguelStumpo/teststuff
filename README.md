# Leegol - Testes automizados
Este projeto consiste num conjunto de testes automizados de vários fluxos do Leegol. 

## Pré-Requisitos
- Ubuntu
__Ubuntu 17.10__

- Maven
__Apache Maven 3.5.0__

- Java 1.8
__openjdk version "1.8.0_171"__
__OpenJDK Runtime Environment (build 1.8.0_171-8u171-b11-0ubuntu0.17.10.1-b11)__
__OpenJDK 64-Bit Server VM (build 25.171-b11, mixed mode)__

- Selenium (como dependência dentro do projeto)
__Selenium 3.12.0__

- OpenCSV (como dependência dentro do projeto)
__OpenCSV 4.1__


### Ferramenta utilizada - __INTELLIJ IDEA__

IntelliJ IDEA 2017.3.2 (Community Edition)
Build #IC-173.4127.27, built on December 25, 2017
JRE: 1.8.0_152-release-1024-b8 amd64
JVM: OpenJDK 64-Bit Server VM by JetBrains s.r.o
Linux 4.13.0-43-generic


## Funções
Este projeto consiste de um anglomerado de testes, que individualmente testam múltiplos fluxos característicos do Leegol.
Cada teste é feito num tempo diferente do seguinte, logo este projeto não ativa testes múltiplos simultâneos.
Estes testes confirmam apenas o cumprimento dos fluxos.

### Tipos de teste

* __Cadastros__
  * Mediador
  * Usuário Normal (Consumo)

* __Solicitações de mediação completas__
  * Condomínio
  * Divórcio
  * Empregador
  * Amigo
  * Vizinho
  * Outra Pessoa

* __Solicitações de mediação incompletas__
  * Empresa
  * Condomínio
  * Divórcio
  * Empregador
  * Familiar
  * Amigo
  * Vizinho
  * Outra pessoa

* __Mediação__

* __Triagem__
  * Aprovação de solicitação
  * Rejeição de solicitação
  * Edição de solicitação
  * Criação de cupon

### Anglomerados de Teste
Estes farão um conjunto de testes, definidos pelos tipos.

* __Todos__
  * Solicitações completas
  * Solicitações incompletas
  * Mediação
  * Cadastro
  * Triagem

## Como rodar:
* Todos
  1. Inicializar o IntelliJ IDEA
  2. Rodar Classe "All tests"

* Teste individual
  1. Inicializar o IntelliJ IDEA
  2. Remover/Ocultar Classe do tipo de teste (EX: teste.main(); -> //teste.main();)
  3. Ir à respetiva classe e fazer do método "public static void main()" para "public static void main(String[] args)"
  4. Rodar a classe
  5. Reverter todas as alterações anteriores quando o teste for concluído.

## Notas
- Às vezes um input de data terá o primeiro dígito do código posto no fim, o que torna o formulário respetivo incompleto, o que interrompe o fluxo.

- No estado atual os testes apenas podem ser feitos todos de uma vez, mas pode especificar-se o teste ao alterar o método da classe respetiva para " public static void main(String[] args) ".

- Os testes atualmente não salvam tempo de desempenho ou erros que não interrompem o fluxo. Atualmente são apenas úteis para notar problemas que interrompem o fluxo.

##¯\_(ツ)_/¯

 
