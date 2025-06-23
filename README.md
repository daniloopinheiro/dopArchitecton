# 🏛️ dopArchitecton

**Coleção prática de arquiteturas backend** com diferentes níveis de complexidade, projetadas para demonstrar padrões reais utilizados em aplicações corporativas modernas.  

O `dopArchitecton` é uma iniciativa educacional e técnica para centralizar **modelos de referência arquitetural**, desde o **monolito modular** até arquiteturas **baseadas em eventos**, **microserviços distribuídos**, **serverless** e muito mais.

---

## 📚 Índice

1. [Objetivo](#objetivo)  
2. [Arquiteturas Disponíveis](#arquiteturas-disponíveis)  
3. [Instalação](#instalação)  
4. [Como Usar](#como-usar)  
5. [Organização de Diretórios](#organização-de-diretórios)  
6. [Contribuições](#contribuições)  
7. [Licença](#licença)  
8. [Contato](#contato)

---

## 🎯 Objetivo

Este repositório foi criado para profissionais, estudantes e equipes que desejam:

- Entender e comparar **diferentes estilos arquiteturais**
- Aplicar boas práticas como **DDD**, **Clean Architecture**, **Event-Driven Design**
- Usar tecnologias como **mensageria, observabilidade, CI/CD**
- Adotar uma abordagem evolutiva de arquitetura (Monolito → Microsserviços → Event-Driven)

Cada projeto é independente e documentado individualmente, com foco em **clareza, escalabilidade e modularidade**.

---

## 🧱 Arquiteturas Disponíveis

| Projeto                           | Tipo de Arquitetura             | Descrição |
|----------------------------------|----------------------------------|-----------|
| `dopArchitecton.Monolithic`      | Monolito Modular                 | Estrutura simples, modular, baseada em camadas |
| `dopArchitecton.Layered`         | Arquitetura em Camadas           | Separação tradicional em UI, Application, Domain, Infra |
| `dopArchitecton.Hexagonal`       | Arquitetura Hexagonal (Ports & Adapters) | Alta desacoplagem entre núcleo e infraestrutura |
| `dopArchitecton.CQRS`            | CQRS + Event Sourcing            | Separação de leitura/escrita + persistência de eventos |
| `dopArchitecton.Microservices`   | Microserviços distribuídos       | Serviços independentes com mensageria assíncrona |
| `dopArchitecton.EventDriven`     | Baseada em Eventos               | Comunicação reativa e desacoplada via EventBus |
| `dopArchitecton.Serverless`      | Functions & Event Grid           | Aplicações elásticas e desacopladas em nuvem |
| `dopArchitecton.Orchestrated`    | Orquestração com Saga / Workflow | Coordenação entre múltiplos serviços/domínios |

---

## 🚀 Instalação

### Pré-requisitos

* [.NET 7 SDK](https://dotnet.microsoft.com/en-us/download)
* [Git](https://git-scm.com)
* [Docker](https://www.docker.com) & [Docker Compose](https://docs.docker.com/compose/)
* **Opcional**: Azure CLI, AWS CLI (para arquiteturas cloud-native)

### Clonando o repositório

```bash
git clone https://github.com/daniloopinheiro/dopArchitecton.git
cd dopArchitecton
````

---

## 🧪 Como Usar

### Executar arquitetura monolítica:

```bash
cd dopArchitecton.Monolithic
dotnet build
dotnet run
```

A aplicação estará disponível em: `https://localhost:5001`

Swagger (se habilitado): `https://localhost:5001/swagger`

### Rodar testes

```bash
dotnet test
```

---

## 🧭 Organização de Diretórios

```bash
dopArchitecton/
│
├── dopArchitecton.Monolithic/         # Monolito modular com separação em camadas
├── dopArchitecton.Layered/            # Arquitetura clássica em camadas
├── dopArchitecton.Hexagonal/          # Ports & Adapters (adaptadores de entrada/saída)
├── dopArchitecton.CQRS/               # Separação entre comandos e consultas
├── dopArchitecton.Microservices/      # Microserviços independentes com event broker
├── dopArchitecton.EventDriven/        # Baseada em eventos com EventBus
├── dopArchitecton.Serverless/         # Functions e eventos cloud (Azure, AWS)
├── dopArchitecton.Orchestrated/       # Orquestração e coordenação de fluxos
│
├── docker-compose.yml                 # Infraestrutura compartilhada (Postgres, Kafka etc)
├── LICENSE
└── README.md
```

---

## 🤝 Contribuições

Você é bem-vindo para:

* Sugerir novas arquiteturas
* Melhorar a implementação atual
* Corrigir erros
* Adicionar testes e documentações

### Para contribuir:

1. Fork este repositório
2. Crie uma branch: `git checkout -b feature/nova-arquitetura`
3. Faça o commit: `git commit -m 'feat: nova arquitetura'`
4. Push: `git push origin feature/nova-arquitetura`
5. Abra um Pull Request 🚀

---

## 📄 Licença

Este projeto está sob a [Licença MIT](LICENSE).

---

## 👋 Contato

Se tiver dúvidas, sugestões ou quiser colaborar:

* **Pessoal**: [daniloopro@gmail.com](mailto:daniloopro@gmail.com)
* **Empresarial**: [devsfree@devsfree.com.br](mailto:devsfree@devsfree.com.br)
* **Consultoria**: [contato@dopme.io](mailto:contato@dopme.io)
* **LinkedIn**: [Danilo O. Pinheiro](https://www.linkedin.com/in/daniloopinheiro)

---

> Desenvolvido por **Danilo O. Pinheiro** • [DevsFree](https://devsfree.com.br) • [dopme.io](https://dopme.io)
