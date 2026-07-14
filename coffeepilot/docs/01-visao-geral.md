# CoffeePilot

## 1. Introdução

O CoffeePilot é uma plataforma SaaS para gestão de cafeterias, projetada para centralizar as principais operações do negócio em um único sistema. A plataforma permite gerenciar cardápio, ingredientes, estoque, pedidos, mesas, clientes e indicadores de desempenho de forma integrada.

Este projeto está sendo desenvolvido como parte do meu portfólio de Engenharia de Software, com o objetivo de aplicar boas práticas de desenvolvimento, arquitetura de software e tecnologias amplamente utilizadas no ecossistema Java em um cenário baseado em necessidades reais de negócio.

## 2. Visão Geral

O CoffeePilot será uma plataforma SaaS (Software as a Service) voltada para a gestão operacional de cafeterias. Cada estabelecimento possuirá um ambiente exclusivo dentro da plataforma, garantindo o isolamento e a segurança de seus dados.

A plataforma será composta por módulos integrados responsáveis por diferentes áreas do negócio, permitindo que todas as informações da cafeteria sejam centralizadas em um único sistema. Entre esses módulos estão:

- Autenticação e controle de acesso;
- Gestão de usuários e funcionários;
- Cardápio e produtos;
- Ingredientes e receitas;
- Controle de estoque;
- Pedidos e mesas;
- Cadastro de clientes;
- Programa de fidelidade;
- Financeiro;
- Dashboards e indicadores de desempenho.

Os módulos compartilharão informações entre si para automatizar processos operacionais. Como exemplo, ao concluir um pedido, o sistema poderá atualizar automaticamente o estoque de ingredientes utilizados na preparação dos produtos, registrar a venda no módulo financeiro e atualizar o histórico do cliente.

O projeto será desenvolvido seguindo uma arquitetura em camadas, utilizando uma API REST como núcleo da aplicação e um frontend web responsável pela interface com os usuários. A solução também será planejada para permitir futuras evoluções, como integração com serviços externos, mecanismos de cache, mensageria e novas funcionalidades sem comprometer a arquitetura existente.

## 3. O Problema

A operação diária de uma cafeteria envolve diversas atividades que precisam funcionar de forma integrada para garantir um atendimento eficiente e uma gestão saudável do negócio. Entretanto, é comum que pequenos estabelecimentos utilizem ferramentas diferentes para controlar cada parte da operação, como planilhas, anotações em papel, aplicativos de mensagens e sistemas isolados.

Essa fragmentação das informações dificulta a tomada de decisão e aumenta a probabilidade de erros operacionais. Um pedido pode ser registrado corretamente, mas o estoque não ser atualizado. Um ingrediente pode acabar durante o expediente sem que exista qualquer alerta prévio. Da mesma forma, torna-se difícil acompanhar quais produtos possuem maior saída, quais clientes são recorrentes ou qual é o desempenho financeiro da cafeteria ao longo do mês.

Outro desafio está no controle dos ingredientes utilizados na preparação das bebidas e alimentos. Em muitos casos, o estoque é atualizado manualmente, sem considerar a quantidade exata consumida em cada receita, o que pode gerar divergências entre o estoque físico e o estoque registrado no sistema.

Além disso, a ausência de indicadores consolidados limita a capacidade dos gestores de identificar oportunidades de melhoria, controlar desperdícios e planejar o crescimento do negócio com base em dados confiáveis.

## 4. A Solução

O CoffeePilot foi idealizado para centralizar toda a operação de uma cafeteria em uma única plataforma, permitindo que os diferentes setores do negócio compartilhem informações de forma integrada.

A plataforma deverá oferecer módulos especializados para gerenciamento de cardápio, ingredientes, estoque, pedidos, mesas, clientes, usuários e indicadores de desempenho, reduzindo a necessidade de controles paralelos e diminuindo a ocorrência de erros operacionais.

Um dos principais diferenciais do sistema será o controle automatizado de ingredientes por meio das receitas cadastradas para cada produto. Ao concluir um pedido, o sistema poderá identificar os ingredientes utilizados, atualizar automaticamente o estoque e registrar a movimentação correspondente, proporcionando maior precisão no controle dos insumos.

Além da automação operacional, o CoffeePilot buscará fornecer informações estratégicas por meio de dashboards e relatórios que auxiliem gestores na tomada de decisão, permitindo acompanhar indicadores como faturamento, ticket médio, produtos mais vendidos e níveis de estoque.

A arquitetura do sistema também será planejada para suportar futuras evoluções, permitindo a incorporação de novas funcionalidades e integrações sem comprometer a organização e a escalabilidade da aplicação.

| Problema                         | Como o CoffeePilot resolve                                         |
| -------------------------------- | ------------------------------------------------------------------ |
| Controle manual de estoque       | Baixa automática de ingredientes através das receitas dos produtos |
| Informações descentralizadas     | Centralização de todos os módulos em uma única plataforma          |
| Dificuldade na gestão financeira | Dashboards e indicadores em tempo real                             |
| Falta de histórico dos clientes  | Cadastro completo e histórico de pedidos                           |
| Pouca visibilidade do desempenho | Relatórios e métricas operacionais                                 |

## 5. Público-alvo

O CoffeePilot foi concebido para atender cafeterias de pequeno e médio porte que buscam centralizar a gestão operacional em uma única plataforma, substituindo controles manuais e processos descentralizados por uma solução integrada.

O sistema é direcionado principalmente a estabelecimentos que necessitam de maior controle sobre estoque, pedidos, cardápio, clientes e indicadores financeiros, mas que não possuem recursos ou necessidade de investir em soluções empresariais complexas e de alto custo.

Por ser uma plataforma SaaS, o CoffeePilot permitirá que diferentes cafeterias utilizem o sistema simultaneamente, cada uma em um ambiente exclusivo e com seus próprios dados, usuários e configurações.

Embora o foco inicial esteja nas cafeterias, a arquitetura da plataforma será projetada de forma modular, possibilitando futuras adaptações para outros negócios do setor de alimentação.

### Perfil dos clientes

| Segmento | Aplicação |
|-----------|-----------|
| Cafeterias independentes | Gestão completa da operação diária. |
| Pequenas redes de cafeterias | Administração centralizada de diferentes unidades (evolução futura). |
| Coffee shops | Controle de produtos, pedidos e estoque. |
| Cafés em livrarias | Organização da operação integrada ao estabelecimento. |
| Cafés em coworkings | Controle de vendas, clientes recorrentes e indicadores de desempenho. |

## 6. Objetivos do Projeto

O desenvolvimento do CoffeePilot possui dois objetivos complementares: criar uma solução capaz de atender às necessidades operacionais de cafeterias e desenvolver um projeto que siga práticas modernas de Engenharia de Software.

### 6.1 Objetivo do Produto

Desenvolver uma plataforma SaaS para centralizar a gestão operacional de cafeterias, reunindo em um único sistema os principais processos do negócio, como controle de estoque, gestão de pedidos, cardápio, clientes, financeiro e indicadores de desempenho.

O sistema deverá contribuir para a redução de erros operacionais, otimização de processos e melhoria da tomada de decisão por meio da integração entre seus módulos.

### 6.2 Objetivo Técnico

Desenvolver um projeto de portfólio inspirado em cenários reais do mercado de software, aplicando princípios de arquitetura, organização de código, documentação, testes, versionamento e desenvolvimento incremental.

O projeto buscará refletir práticas utilizadas em equipes profissionais, priorizando qualidade, escalabilidade, manutenção e evolução contínua da aplicação.

## 7. Escopo Geral

O escopo do CoffeePilot contempla o desenvolvimento de uma plataforma web para gestão operacional de cafeterias, com foco em pequenos e médios estabelecimentos.

A versão inicial do projeto será desenvolvida com o objetivo de oferecer uma solução completa para as principais necessidades do dia a dia de uma cafeteria, priorizando funcionalidades que agreguem valor à operação e demonstrem uma arquitetura sólida, escalável e de fácil manutenção.

O sistema será composto por módulos integrados, permitindo que diferentes áreas da operação compartilhem informações de forma automática e consistente.

Nesta primeira versão, o projeto terá como foco a implementação dos seguintes módulos:

- Autenticação e controle de acesso;
- Gestão da cafeteria;
- Usuários e permissões;
- Cardápio e produtos;
- Ingredientes e receitas;
- Controle de estoque;
- Pedidos;
- Mesas;
- Clientes;
- Financeiro;
- Dashboard gerencial.

Embora a arquitetura seja planejada para suportar futuras expansões, algumas funcionalidades permanecerão fora do escopo inicial do projeto e poderão ser desenvolvidas em versões posteriores.

## 8. Módulos da Plataforma

O CoffeePilot será composto por módulos integrados que contemplam as principais áreas da operação de uma cafeteria. Cada módulo será detalhado em documentos específicos ao longo do desenvolvimento do projeto.

| Módulo | Objetivo |
|--------|----------|
| Autenticação e Controle de Acesso | Gerenciar autenticação, autorização e segurança dos usuários. |
| Gestão da Cafeteria | Administrar as informações da cafeteria e suas configurações. |
| Usuários e Funcionários | Gerenciar usuários, perfis e permissões de acesso. |
| Cardápio | Cadastrar e organizar os produtos comercializados. |
| Ingredientes e Receitas | Definir ingredientes e receitas utilizadas nos produtos. |
| Controle de Estoque | Controlar entradas, saídas e disponibilidade dos ingredientes. |
| Pedidos | Gerenciar o fluxo completo dos pedidos realizados. |
| Mesas | Controlar ocupação e organização das mesas da cafeteria. |
| Clientes | Registrar clientes e acompanhar seu histórico de consumo. |
| Financeiro | Gerenciar receitas, despesas e fluxo de caixa. |
| Dashboard Gerencial | Apresentar indicadores para apoio à tomada de decisão. |

## 9. Diferenciais do Projeto

O CoffeePilot foi concebido para ser mais do que um sistema de cadastro e gerenciamento de informações. Seu objetivo é integrar diferentes áreas da operação de uma cafeteria, automatizando processos e fornecendo informações estratégicas para apoiar a tomada de decisão.

Os principais diferenciais planejados para a plataforma são apresentados a seguir.

### Controle de Estoque Baseado em Receitas

Cada produto do cardápio poderá possuir uma receita composta por ingredientes e suas respectivas quantidades.

Ao concluir um pedido, o sistema calculará automaticamente o consumo de cada ingrediente utilizado na preparação dos produtos, atualizando o estoque sem necessidade de intervenção manual.

Essa abordagem reduz erros operacionais e proporciona maior precisão no controle dos insumos.

---

### Integração entre os Módulos

Todos os módulos compartilharão informações entre si.

Uma ação realizada em determinado módulo poderá refletir automaticamente em outros, reduzindo retrabalho e garantindo consistência dos dados.

Como exemplo:

Pedido concluído

  ↓

Baixa automática do estoque

  ↓

Registro da venda

  ↓

Atualização do histórico do cliente

  ↓
  
Atualização do dashboard gerencial

---

### Plataforma SaaS

O CoffeePilot será desenvolvido seguindo o modelo Software as a Service (SaaS).

Cada cafeteria possuirá seu próprio ambiente, garantindo isolamento de dados, segurança e possibilidade de expansão para múltiplos clientes utilizando uma única aplicação.

---

### Arquitetura Planejada para Evolução

Desde sua concepção, a arquitetura será organizada para permitir o crescimento gradual da plataforma.

Novas funcionalidades poderão ser incorporadas sem necessidade de grandes alterações estruturais, favorecendo a manutenção e a escalabilidade do sistema.

---

### Desenvolvimento Baseado em Documentação

Todo o desenvolvimento será conduzido a partir de documentação previamente definida, incluindo visão do produto, requisitos, regras de negócio, arquitetura, modelagem de dados e roadmap.

Essa abordagem busca reduzir retrabalho e aproximar o processo de desenvolvimento das práticas adotadas em equipes profissionais de Engenharia de Software.

---

### Evolução Contínua do Produto

O CoffeePilot será desenvolvido de forma incremental.

Cada versão entregará novas funcionalidades e melhorias, mantendo um histórico claro da evolução do sistema e permitindo a validação contínua da arquitetura e das decisões de projeto.

## 10. Tecnologias Utilizadas

O CoffeePilot será desenvolvido utilizando tecnologias amplamente adotadas no mercado de desenvolvimento de software. A escolha de cada ferramenta busca equilibrar produtividade, escalabilidade, facilidade de manutenção e aderência às boas práticas de Engenharia de Software.

### Backend

O backend será responsável pela implementação da regra de negócio, autenticação, autorização, validação dos dados e disponibilização da API REST consumida pelo frontend.

| Tecnologia | Finalidade |
|------------|------------|
| Java 26 | Linguagem principal da aplicação. |
| Spring Boot | Framework para construção da API REST. |
| Spring Security | Autenticação, autorização e segurança da aplicação. |
| Spring Data JPA | Persistência e acesso aos dados. |
| Hibernate | Implementação do JPA e mapeamento objeto-relacional. |
| PostgreSQL | Banco de dados relacional. |
| Flyway | Controle de versionamento das migrações do banco de dados. |
| JWT | Autenticação baseada em tokens. |
| Bean Validation | Validação dos dados de entrada da API. |
| OpenAPI / Swagger | Documentação automática da API REST. |
| JUnit 5 | Testes unitários. |
| Mockito | Criação de mocks para testes automatizados. |

---

### Frontend

O frontend será responsável pela interface com o usuário, consumindo os serviços disponibilizados pela API REST.

| Tecnologia | Finalidade |
|------------|------------|
| React | Biblioteca para construção da interface. |
| TypeScript | Superset do JavaScript com tipagem estática. |
| Vite | Ferramenta para criação e execução do projeto React. |
| React Router | Gerenciamento das rotas da aplicação. |
| Axios | Comunicação com a API REST. |
| TanStack Query | Gerenciamento de estado assíncrono e cache das requisições. |

---

### DevOps

As ferramentas de DevOps serão incorporadas gradualmente conforme a evolução do projeto.

| Tecnologia | Finalidade |
|------------|------------|
| Docker | Padronização do ambiente de desenvolvimento e execução da aplicação. |
| Docker Compose | Orquestração dos serviços da aplicação durante o desenvolvimento. |
| GitHub Actions | Integração contínua (CI) e automação de processos. |
| Nginx | Servidor web e proxy reverso para publicação da aplicação. |

---

### Evoluções Futuras

Algumas tecnologias serão incorporadas em versões posteriores do CoffeePilot para suportar novas funcionalidades e melhorias de desempenho.

| Tecnologia | Objetivo |
|------------|----------|
| RabbitMQ | Comunicação assíncrona entre módulos. |
| Redis | Cache e otimização de desempenho. |
| WebSocket | Atualizações em tempo real para pedidos e dashboards. |

## 11. Arquitetura em Alto Nível

O CoffeePilot será desenvolvido seguindo uma arquitetura cliente-servidor, onde a interface web será responsável pela interação com os usuários e consumirá uma API REST responsável por toda a regra de negócio da aplicação.

A separação entre frontend e backend permitirá que cada componente evolua de forma independente, facilitando a manutenção, a escalabilidade e futuras integrações com outras aplicações ou clientes.

A persistência dos dados será realizada em um banco de dados PostgreSQL, enquanto ferramentas de infraestrutura serão utilizadas para padronizar o ambiente de desenvolvimento, automatizar processos e facilitar o deploy da aplicação.

A arquitetura também será planejada para suportar futuras evoluções, como mecanismos de cache, mensageria, comunicação em tempo real e integração com serviços externos, sem comprometer a organização do sistema.

## 12. Roadmap do Produto

O CoffeePilot será desenvolvido de forma incremental, permitindo que novas funcionalidades sejam incorporadas conforme a evolução do projeto.

Cada versão terá objetivos bem definidos, priorizando a entrega de valor contínua, a qualidade da arquitetura e a evolução gradual da plataforma.

O roadmap apresentado a seguir representa o planejamento inicial do projeto e poderá sofrer alterações conforme novas necessidades, aprendizados e oportunidades de melhoria forem identificados durante o desenvolvimento.

### Versão 0.1 — Primeira Versão Funcional

Objetivo: desenvolver a base da plataforma e implementar os principais processos operacionais de uma cafeteria.

Funcionalidades previstas:

- Autenticação e controle de acesso;
- Gestão de usuários;
- Gestão da cafeteria;
- Cardápio e produtos;
- Ingredientes;
- Receitas dos produtos;
- Controle automático de estoque;
- Gestão de pedidos;
- Documentação da API;
- Testes iniciais.

---

### Versão 0.5 — Evolução Operacional

Objetivo: ampliar as funcionalidades voltadas para a operação diária da cafeteria.

Funcionalidades previstas:

- Gestão de mesas;
- Cadastro de clientes;
- Dashboard gerencial;
- Histórico de pedidos;
- Melhorias na interface;
- Upload de imagens dos produtos.

---

### Versão 1.0 — Primeira Versão Estável

Objetivo: consolidar a plataforma como uma solução completa para gestão de cafeterias.

Funcionalidades previstas:

- Módulo financeiro;
- Relatórios gerenciais;
- Programa de fidelidade;
- Melhorias de desempenho;
- Cobertura ampliada de testes;
- Deploy em ambiente de produção.

---

### Versão 2.0 — Escalabilidade e Integrações

Objetivo: preparar a plataforma para cenários mais complexos e maior escalabilidade.

Funcionalidades previstas:

- Cache com Redis;
- Comunicação assíncrona com RabbitMQ;
- Atualizações em tempo real com WebSocket;
- Integrações com serviços externos;
- API pública;
- Auditoria;
- Melhorias de segurança;
- Otimizações de performance.

## 13. Glossário

| Termo | Definição |
|--------|-----------|
| SaaS (Software as a Service) | Modelo de software disponibilizado pela internet, onde diferentes clientes utilizam a mesma aplicação sem necessidade de instalação local. |
| Multi-tenancy | Arquitetura onde uma única aplicação atende diferentes clientes (cafeterias), mantendo seus dados isolados. |
| API | Interface que permite a comunicação entre diferentes sistemas ou aplicações. |
| API REST | Interface baseada em princípios REST, utilizada para comunicação entre o frontend e o backend por meio de requisições HTTP. |
| Frontend | Camada da aplicação responsável pela interface e interação com o usuário. |
| Backend | Camada da aplicação responsável pela implementação da regra de negócio, autenticação, autorização, validações, processamento das requisições e comunicação com o banco de dados. |
| Arquitetura em Camadas | Organização da aplicação em camadas com responsabilidades bem definidas, como apresentação, negócio e persistência. |
| Banco de Dados | Sistema responsável pelo armazenamento persistente, organização e recuperação das informações da aplicação. |
| ORM (Object-Relational Mapping) | Técnica que permite mapear objetos da aplicação para tabelas do banco de dados. |
| Migração de Banco de Dados | Processo de criação e versionamento da estrutura do banco de dados ao longo da evolução do projeto. |
| Dashboard | Painel que reúne indicadores e métricas para auxiliar na tomada de decisão. |
| Cardápio | Conjunto de produtos comercializados pela cafeteria. |
| Produto | Item disponível para venda, como bebidas, alimentos e sobremesas. |
| Ingrediente | Insumo utilizado na preparação de um ou mais produtos do cardápio. |
| Receita | Definição da quantidade de ingredientes necessária para produzir um determinado produto. |
| Estoque | Controle da quantidade disponível de ingredientes utilizados pela cafeteria. |
| Pedido | Solicitação realizada por um cliente contendo um ou mais produtos. |
| Cliente | Pessoa que realiza compras na cafeteria e pode possuir histórico de pedidos e participação em programas de fidelidade. |
| JWT (JSON Web Token) | Token utilizado para autenticação e autorização dos usuários da plataforma. |
| Docker | Plataforma utilizada para empacotar e executar aplicações em contêineres, garantindo ambientes consistentes. |
| Docker Compose | Ferramenta para definir e executar múltiplos serviços da aplicação por meio de um único arquivo de configuração. |
| CI/CD (Continuous Integration / Continuous Delivery) | Conjunto de práticas para automatizar a integração, testes e entrega da aplicação. |
| Deploy | Processo de publicação de uma nova versão da aplicação em um ambiente de execução. |
| Cache | Técnica utilizada para armazenar temporariamente dados acessados com frequência, melhorando o desempenho da aplicação. |
| Mensageria | Comunicação assíncrona entre sistemas ou módulos por meio de filas de mensagens. |
| RabbitMQ | Sistema de mensageria utilizado para processamento assíncrono e desacoplamento entre componentes da aplicação. |
| Redis | Banco de dados em memória utilizado principalmente para cache e otimização de desempenho. |
| WebSocket | Protocolo de comunicação bidirecional em tempo real entre cliente e servidor. |
| Flyway | Ferramenta responsável pelo controle de versão e aplicação das migrações do banco de dados. |
| MVP (Minimum Viable Product) | Primeira versão funcional do produto contendo apenas as funcionalidades essenciais. |
| Roadmap | Planejamento que descreve a evolução prevista do produto ao longo das versões. |