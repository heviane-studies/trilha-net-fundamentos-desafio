 # 🅿️ Estacionamento de veículos

<p align="center">
  <a href="https://github.com/heviane-studies/trilha-net-fundamentos-desafio/actions/workflows/dotnet-ci.yml"><img alt="Build Status" src="https://github.com/heviane-studies/trilha-net-fundamentos-desafio/actions/workflows/dotnet-ci.yml/badge.svg" /></a>
  <a href="https://github.com/heviane-studies/trilha-net-fundamentos-desafio/releases"><img alt="Latest Release" src="https://img.shields.io/github/v/release/heviane-studies/trilha-net-fundamentos-desafio?style=flat-square&color=success" /></a>
  <a href="../LICENSE"><img alt="License" src="https://img.shields.io/github/license/heviane-studies/trilha-net-fundamentos-desafio?style=flat-square&color=blue" /></a>
  <a href="https://github.com/heviane-studies/trilha-net-fundamentos-desafio/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/heviane-studies/trilha-net-fundamentos-desafio?style=flat-square&color=blueviolet" /></a>
  <img alt="Contributions Welcome" src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square" />
</p>

## 📋 Descrição do projeto

Este projeto é uma aplicação de console em .NET que simula um sistema de gerenciamento de estacionamento. Desenvolvido como um desafio prático, ele aplica conceitos fundamentais de C# e da plataforma .NET, incluindo programação orientada a objetos, manipulação de coleções e interação com o usuário via terminal.

O sistema permite realizar operações essenciais como registrar a entrada de veículos, processar a saída com cálculo de custos e listar os veículos presentes, servindo como uma base sólida para a implementação de funcionalidades mais avançadas.

## ✨ Funcionalidades

A aplicação oferece as seguintes funcionalidades essenciais para a gestão de um estacionamento:

- **Cadastrar Veículo**:
  - Permite registrar um novo veículo no estacionamento através de sua placa.
  - Inclui uma validação para impedir o cadastro de placas duplicadas, garantindo a integridade dos dados.

- **Remover Veículo e Calcular Custo**:
  - Remove um veículo registrado do estacionamento.
  - Solicita a quantidade de horas que o veículo permaneceu estacionado.
  - Calcula e exibe o valor total a ser pago, com base no preço inicial e no preço por hora definidos no início da execução.

- **Listar Veículos**:
  - Exibe uma lista com as placas de todos os veículos que estão atualmente no estacionamento.

<!-- 
## Layout ou Deploy da Aplicação :dash:

> Link do deploy da aplicação. Exemplo com netlify: https://certificates-for-everyone-womakerscode.netlify.app/

...

Se ainda não houver deploy, insira capturas de tela da aplicação ou gifs
-->

## 🛠️ Pré-requisitos

Para clonar e executar este projeto localmente, você precisará ter as seguintes ferramentas instaladas em sua máquina:

- **[.NET 9.0 SDK](https://dotnet.microsoft.com/en-us/download)**: Essencial para compilar e executar a aplicação e os testes.
- **[Git](https://git-scm.com/)**: Necessário para clonar o repositório.
- **[Docker](https://www.docker.com/products/docker-desktop/)**: Opcional, mas necessário para construir e executar a aplicação via container.

  ### Recomendado

  - Um editor de código como o **[Visual Studio Code](https://code.visualstudio.com/)** com a extensão [C# Dev Kit](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csdevkit).

## :arrow_forward: Como rodar a aplicação

No terminal, execute os comandos abaixo:

```bash
## Clone o projeto:
git clone git@github.com:heviane-studies/trilha-net-fundamentos-desafio.git

## Entre na pasta do projeto:
cd trilha-net-fundamentos-desafio/Parking 
```

### Rodar a aplicação sem Docker

```bash
dotnet run
```

### Rodar a aplicação com Docker

Com o Docker instalado e executando, você pode construir e executar a aplicação em um ambiente containerizado, garantindo consistência e isolamento.

```bash
# construa a imagem Docker: 
docker build -t parking-app .

# Execute o container de forma interativa:
# Flag -it para alocar um terminal interativo, essencial para uma aplicação de console
# Flag --rm para remover o container automaticamente após a sua execução.
docker run -it --rm parking-app
```

<!-- TODO: Dica: clone o próprio projeto e verfique se o passo a passo funciona. -->

## 🧪 Como rodar os testes

Para garantir a qualidade e o correto funcionamento do projeto, a aplicação conta com uma suíte de testes unitários. As instruções detalhadas para executar os testes estão disponíveis no [**README do projeto de testes**](../Parking.Tests/README.md#4-como-executar-os-testes-).

<!--
## Casos de Uso

Explique com mais detalhes como a sua aplicação poderia ser utilizada. O uso de **gifs** aqui seria bem interessante.

Exemplo: Caso a sua aplicação tenha alguma funcionalidade de login apresente neste tópico os dados necessários para acessá-la.

## JSON :floppy_disk:

### Usuários:

|name|email|password|token|avatar|
| -------- |-------- |-------- |-------- |-------- |
|Lais Lima|laislima98@hotmail.com|lais123|true|https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcS9-U_HbQAipum9lWln3APcBIwng7T46hdBA42EJv8Hf6Z4fDT3&usqp=CAU|

...

Se quiser, coloque uma amostra do banco de dados

## Iniciando/Configurando banco de dados

Se for necessário configurar algo antes de iniciar o banco de dados insira os comandos a serem executados

## Linguagens, dependencias e libs utilizadas :books:

- [React](https://pt-br.reactjs.org/docs/create-a-new-react-app.html)
- [React PDF](https://react-pdf.org/)

...

Liste as tecnologias utilizadas no projeto que **não** forem reconhecidas pelo Github

## Resolvendo Problemas :exclamation:

Em [issues](https://github.com/heviane-studies/trilha-net-fundamentos-desafio/issues) foram abertos alguns problemas gerados durante o desenvolvimento desse projeto e como foram resolvidos.
-->

## :memo: Próximos passos

- [x] Implementar o uso de **containers** com **Docker**.
  - Garante um ambiente de execução consistente, portátil e simplifica o setup para novos desenvolvedores.
  - Isola a aplicação e suas dependências, evitando conflitos com o ambiente da máquina hospedeira.
  - Utiliza um `Dockerfile` multi-stage para criar uma imagem final leve e otimizada, contendo apenas o necessário para a execução.
- [X] Implementar **projeto de testes unitários** com **XUnit**.
  - Garante a qualidade, robustez e manutenibilidade da lógica de negócio.
  - Facilita futuras manutenções e refatorações, garantindo que o comportamento esperado não seja quebrado.
  - Exigiu a refatoração da aplicação para separar responsabilidades (SoC), uma prática fundamental da arquitetura de software limpa.
- [X] Implementar **Integração Contínua (CI)** com **GitHub Actions**.
  - Garante que os testes sejam executados automaticamente toda vez que um novo código é enviado para o repositório (a cada `push` ou em cada `Pull Request`).
  - Impede código com bugs ou que quebre funcionalidades existentes seja integrado à branch principal (main).
  - Desenvolvedores e contribuidores sabem imediatamente se uma alteração causou um problema.
  - Criar um workflow que compila o projeto e executa o `dotnet test`.
- [ ] Implementar o uso de **banco de dados**
- [ ] Implementar **autenticação**
- [ ] Criar uma **versão web**
  - [ ] Designer: Identidade visual, design system, wireframe, protótipo, etc.
  - [ ] Frontend: User interface.
- [ ] Criar uma **versão mobile** para android.
- [ ] Criar uma **versão mobile** para ios.
- [ ] Criar uma **versão mobile** para tablet.
- [ ] Criar uma **versão mobile** para desktop.

## :octocat: Desenvolvedores e Contribuintes

| [<img src="https://heviane.github.io/image-gallery/Profile-heviane-v2.PNG" width=115><br><sub>Heviane Bastos</sub>](https://github.com/heviane) |
| :---: |

## 📜 Licença

The [MIT License](../LICENSE) (MIT)

Copyright :copyright: 2025 - Estacionamento de veículos
