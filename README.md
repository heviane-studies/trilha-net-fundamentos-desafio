# 🎓 Trilha .NET: Fundamentos e Desafios

<p align="center">
  <a href="https://github.com/heviane/trilha-net-fundamentos-desafio/actions/workflows/dotnet-ci.yml"><img alt="Build Status" src="https://img.shields.io/github/actions/workflow/status/heviane/trilha-net-fundamentos-desafio/dotnet-ci.yml?branch=main&style=for-the-badge&label=CI"></a>
  <a href="https://github.com/heviane/trilha-net-fundamentos-desafio/releases"><img alt="Latest Release" src="https://img.shields.io/github/v/release/heviane/trilha-net-fundamentos-desafio?style=for-the-badge&color=success"></a>
  <a href="./LICENSE"><img alt="License" src="https://img.shields.io/github/license/heviane/trilha-net-fundamentos-desafio?style=for-the-badge&color=blue"></a>
  <a href="./.github/CONTRIBUTING.md"><img alt="Contributions Welcome" src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=for-the-badge"></a>
</p>

> Repositório dedicado ao aprendizado e desenvolvimento de desafios da trilha de formação .NET da [Digital Innovation One](https://www.dio.me/).

## 🎯 Sobre o Repositório

Este espaço documenta minha jornada de estudos na trilha de desenvolvimento .NET. Ele serve como um portfólio, contendo as soluções para os desafios propostos, organizados em projetos individuais. O objetivo é aplicar conceitos fundamentais e avançados da plataforma .NET e da linguagem C#, seguindo as melhores práticas de desenvolvimento de software.

## 📂 Projetos Desenvolvidos

Abaixo está a lista de projetos contidos neste repositório. Cada um representa um desafio específico da trilha de aprendizado.

| Projeto | Descrição | Status |
| :--- | :--- | :---: |
| 🅿️ [**Parking**](./Parking/) | Uma aplicação de console para gerenciar um sistema de estacionamento, com testes (xUnit), Docker e CI com GitHub Actions. | ✅ Concluído |
| 🏨 [**Booking**](./Booking/) | Uma aplicação de console para gerenciar um sistema de hospedagem, com testes (xUnit), Docker e CI com GitHub Actions. | ✅ Concluído |
| 📱 [**SmartPhone**](./SmartPhone/) | Uma aplicação de console para gerenciar um sistema de SmartPhone, com testes (xUnit), Docker e CI com GitHub Actions. | ✅ Concluído |
| ... | *Novos desafios serão adicionados aqui.* | 🚧 Em breve |

## 📄 Créditos e Origem dos Desafios

Os projetos neste repositório foram desenvolvidos com base nos desafios de código propostos pela [Digital Innovation One (DIO)](https://www.dio.me/). Os repositórios originais, que serviram como ponto de partida, são:

- **Parking**: [digitalinnovationone/trilha-net-fundamentos-desafio](https://github.com/digitalinnovationone/trilha-net-fundamentos-desafio)
- **Booking**: [digitalinnovationone/trilha-net-explorando-desafio](https://github.com/digitalinnovationone/trilha-net-explorando-desafio)
- **SmartPhone**: [digitalinnovationone/trilha-net-poo-desafio](https://github.com/digitalinnovationone/trilha-net-poo-desafio)

Este repositório representa minha implementação e evolução sobre as propostas iniciais, adicionando testes, automações e outras boas práticas de engenharia de software.

## 🗺️ Roadmap e Padrões de Desenvolvimento

Para garantir a qualidade, consistência e manutenibilidade de todos os desafios, cada projeto neste repositório deve seguir um conjunto de padrões de desenvolvimento.

### Padrões de Qualidade adotados para este Repositório e seus Projetos

- ✅ **Testes Unitários**: Implementar uma suíte de testes com **xUnit** para validar a lógica de negócio das aplicações de console.
- ✅ **Containerização**: Criar um `Dockerfile` para executar a aplicação em um ambiente isolado com **Docker**.
- ✅ **Integração Contínua (CI)**: Configurar um `workflow` no **GitHub Actions** para compilar e testar o código automaticamente.
- ✅ **Release Automatizada**: Configurar um `workflow` para criar releases no GitHub automaticamente, anexando os executáveis compilados (artefatos) para Linux, Windows e macOS.

### Padrões de Qualidade em análise para futuras implementações

- 🚧 **Análise Estática (Linting)**: Implementar verificação de formatação e estilo de código no CI.
- 🚧 **Cobertura de Testes**: Adicionar relatórios de cobertura de testes (ex: Codecov) ao workflow de CI.
- 🚧 **Otimização de Build**: Refatorar o workflow de release para executar builds em paralelo, reduzindo o tempo de execução.

### Funcionalidades em análise para futuras implementações

Além dos padrões de qualidade, as seguintes funcionalidades estão no radar para serem exploradas em projetos futuros ou como evoluções dos desafios atuais:

- [ ] Implementar o uso de **banco de dados** para persistência de dados.
- [ ] Criar uma **versão web** das aplicações utilizando ASP.NET Core.
- [ ] Explorar a criação de **APIs RESTful**.
- [ ] Implementar mecanismos de **autenticação e autorização**.

## 🤝 Como Contribuir

Este é um projeto de código aberto e ficamos felizes em receber contribuições! Se você tem interesse em ajudar, seja corrigindo bugs, propondo novas funcionalidades ou melhorando a documentação, sua ajuda é muito bem-vinda.

1. Leia nosso [**Guia de Contribuição**](./.github/CONTRIBUTING.md) para entender o processo.
2. Observe nosso [**Código de Conduta**](./.github/CODE_OF_CONDUCT.md) para garantir um ambiente colaborativo e respeitoso.
3. Procure por [issues abertas](./issues) para encontrar tarefas em que você pode ajudar.

## :octocat: Desenvolvedores e Contribuintes

| [<img width="80px" align="center" src="https://avatars.githubusercontent.com/heviane"/><br><sub>Heviane Bastos</sub>](https://github.com/heviane) |
| :---: |

## 📜 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

Copyright © 2025 - Heviane Bastos
