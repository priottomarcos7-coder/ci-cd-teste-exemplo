# CI/CD e Qualidade Contínua — Jenkins

## Objetivo

Projeto desenvolvido para praticar integração contínua e execução automatizada de testes em um pipeline de CI/CD.

Neste projeto desenvolvi a configuração de um pipeline com Jenkins para integrar o código versionado no GitHub ao processo de execução dos testes automatizados.

## O que desenvolvi

- Configuração de pipeline utilizando Jenkins.
- Integração do repositório GitHub ao processo de CI/CD.
- Execução automatizada dos testes durante o pipeline.
- Configuração do ambiente necessário para execução com Node.js.
- Investigação e correção de problemas de configuração do Jenkins, Git e dependências.
- Uso do pipeline como mecanismo de apoio à qualidade contínua.

## Tecnologias

- Jenkins
- Git
- GitHub
- Node.js
- JavaScript
- Cypress
- CI/CD

## Pré-requisitos

- Git instalado.
- Node.js instalado.
- Jenkins instalado e configurado.
- Acesso ao repositório GitHub.

## Instalação

Clone o projeto:

```bash
git clone https://github.com/priottomarcos7-coder/ci-cd-teste-exemplo.git
cd ci-cd-teste-exemplo
```

Instale as dependências, quando aplicável:

```bash
npm install
```

## Execução local

Execute os testes conforme os scripts disponíveis no `package.json`. Para projetos Cypress, por exemplo:

```bash
npx cypress run
```

## Execução pelo Jenkins

1. Abra o Jenkins.
2. Crie ou configure um projeto do tipo Pipeline.
3. Aponte o pipeline para o repositório GitHub.
4. Utilize o `Jenkinsfile` presente no projeto.
5. Execute o pipeline.
6. Analise o resultado da etapa de testes.

## Estratégia de CI/CD

A ideia do projeto é inserir a execução de testes no fluxo de entrega para que problemas sejam identificados de forma antecipada, reduzindo o risco de alterações com falhas chegarem às próximas etapas.

## Estrutura principal

```text
Jenkinsfile
package.json
README.md
```

## Resultado esperado

Ao executar o pipeline, o Jenkins deve realizar as etapas configuradas e apresentar o resultado da execução dos testes.

## Repositório

https://github.com/priottomarcos7-coder/ci-cd-teste-exemplo

## Autor

Marcos Priotto

Projeto desenvolvido como parte da formação em Engenharia de Qualidade de Software na EBAC.