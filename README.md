# Sistema CodeFactory

## Descrição do projeto

O Sistema CodeFactory é uma aplicação web simples desenvolvida para a empresa fictícia CodeFactory Solutions. O sistema permite o cadastro e gerenciamento de tarefas de forma simples e organizada.

O projeto também é utilizado para demonstrar a aplicação de práticas de DevOps, como controle de versão com Git e GitHub, utilização de branches, Pull Requests, Docker e Integração Contínua.

## Objetivo

O objetivo do projeto é demonstrar a adoção de práticas DevOps no desenvolvimento de uma aplicação web, buscando tornar o processo de desenvolvimento mais organizado, colaborativo, automatizado e confiável.

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- Git
- GitHub
- Docker
- GitHub Actions

## Estrutura do projeto

```text
Sistema-CodeFactory/
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
├── css/
│   └── style.css
│
├── js/
│   └── script.js
│
├── Dockerfile
├── LICENSE
├── index.html
└── README.md
```

## Instalação

### Pré-requisitos

Para executar o projeto localmente, é necessário ter um navegador web instalado.

Para as etapas de versionamento e containerização, são utilizados:

- Git
- Docker

### Clonar o repositório

```bash
git clone https://github.com/milenapauli/Sistema-CodeFactory.git
```

### Acessar a pasta do projeto

```bash
cd Sistema-CodeFactory
```

## Execução

A aplicação pode ser executada diretamente no navegador.

Basta abrir o arquivo `index.html`.

Também é possível utilizar uma extensão de servidor local, como o Live Server, durante o desenvolvimento.

## Docker

A aplicação também pode ser executada utilizando Docker.

Foi criado um `Dockerfile` utilizando a imagem Nginx para disponibilizar a aplicação web em um container.

Para construir a imagem:

```bash
docker build -t sistema-codefactory .
```

Para executar o container:

```bash
docker run -d --name sistema-codefactory -p 8080:80 sistema-codefactory
```

Após iniciar o container, a aplicação pode ser acessada pelo navegador através de:

```text
http://localhost:8080
```

A utilização do Docker permite padronizar o ambiente de execução da aplicação e facilitar sua reprodução em diferentes ambientes.

## Controle de versão

O projeto utiliza Git e GitHub para controle de versão.

Durante o desenvolvimento foram utilizadas as branches:

- `main`
- `desenvolvimento`
- `tarefas`

Também foram utilizados commits, Pull Requests, merge e resolução de conflitos.

## Integração Contínua

O projeto utiliza GitHub Actions para realizar a Integração Contínua.

O pipeline realiza a validação da estrutura básica do projeto e a construção da imagem Docker.

A execução do pipeline ocorre automaticamente em alterações realizadas nas branches `main` e `desenvolvimento`, bem como em Pull Requests direcionados a essas branches.

## Licença

Este projeto está disponível sob a licença MIT.

A licença completa está disponível no arquivo `LICENSE`.