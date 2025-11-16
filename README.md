# 🚗 AutoGest

## Documentação de Arquitetura de Software

---

### 🚀 Bem-vindo(a) à documentação do Projeto AutoGest!

Este repositório concentra toda a documentação técnica de arquitetura, design e modelagem do software **AutoGest**. Neste espaço, estão reunidos diversos diagramas UML e documentos visuais que explicam a estrutura, o funcionamento e as interações do sistema, oferecendo uma compreensão detalhada e organizada para desenvolvedores, analistas e demais interessados no projeto.

### 📖 Sobre o Sistema

O AutoGest é um software focado em otimizar a gestão de uma autoescola, englobando cadastros de alunos, veículos e instrutores, além do controle de aulas. Com essa solução, busca-se eliminar a necessidade do uso de um sistema que não é agradável ao cliente, melhorando a organização, reduzindo erros da gestão manual e aumentando a eficiência operacional. O sistema também, permitirá um acompanhamento mais preciso das atividades da autoescola, facilitando o agendamento de aulas, a gestão de pagamentos e a comunicação entre alunos e instrutores. Dessa forma, espera-se proporcionar uma experiência mais eficaz para os envolvidos.

### 📚 Índice

- [Sobre o Sistema](#-sobre-o-sistema)
- [Visão Geral da Documentação](#-visão-geral-da-documentação)
- [Diagrama de Arquitetura](#-diagrama-de-arquitetura)
- [Diagrama de Caso de Uso](#-diagrama-de-caso-de-uso)
- [Diagrama de Classe](#-diagrama-de-classe)
- [Diagrama de Componentes](#-diagrama-de-componentes)
- [Diagramas de Comunicação](#-diagramas-de-comunicação)
  - [Comunicação: Cadastro de Aluno (UC-01)](#diagrama-de-comunicação-cadastro-de-aluno-uc-01)
  - [Comunicação: Visualizar Relatórios (UC-09/10)](#diagrama-de-comunicação-visualizar-relatórios-uc-0910)
- [Diagramas de Estados](#-diagramas-de-estados)
  - [Estados: Status de Matrícula do Aluno](#diagrama-de-estados-status-de-matrícula-do-aluno)
  - [Estados: Aula Prática](#diagrama-de-estados-aula-prática)
- [Diagrama de Implantação](#-diagrama-de-implantação)
- [Diagrama de Modelo de Dados](#-diagrama-de-modelo-de-dados)
- [Diagramas de Sequência](#-diagramas-de-sequência)
  - [Sequência: Cadastrar Novo Aluno (UC-01)](#diagrama-de-sequência-cadastrar-novo-aluno-uc-01)
  - [Sequência: Marcar Presença (UC-06)](#diagrama-de-sequência-marcar-presença-uc-06)
  - [Sequência: Visualizar Relatório (UC-09/10)](#diagrama-de-sequência-visualizar-relatório-uc-0910)
  - [Sequência: Agendar Aula Prática (UC-05)](#diagrama-de-sequência-agendar-aula-prática-uc-05)
  - [Sequência: Cadastro de Funcionário (UC-02)](#diagrama-de-sequência-cadastro-de-funcionário-uc-02)
  - [Sequência: Visualizar Agenda (UC-07)](#diagrama-de-sequência-visualizar-agenda-uc-07)


---

### 💡 Visão Geral da Documentação

Nas seções seguintes, cada diagrama é apresentado com uma explicação sobre sua função e significado dentro do contexto do **AutoGest**, permitindo uma compreensão completa da arquitetura e do funcionamento do sistema.

---

### 🏛️ Diagrama de Arquitetura

O diagrama de arquitetura (C4 Nível 2) apresenta a estrutura geral do **AutoGest** em alto nível, exibindo os principais elementos do sistema (aplicações web, serviços backend, bancos de dados) e como eles se relacionam. Oferece uma perspectiva ampla sobre a organização arquitetural da solução.

![Diagrama de Arquitetura](ImagesPlantUML/arquitetura.png)

---

### 👥 Diagrama de Caso de Uso

Demonstra as principais funcionalidades do **AutoGest** através dos casos de uso, mapeando os atores envolvidos (Administrador, Funcionário, Instrutor) e as ações que cada um pode realizar no sistema, definindo o comportamento esperado do ponto de vista do usuário.

![Diagrama de Caso de Uso](ImagesPlantUML/casosdeuso.png)

---

### 🧱 Diagrama de Classe

Expõe a modelagem orientada a objetos do sistema, apresentando todas as classes com seus respectivos atributos, operações e as conexões estáticas (associações, heranças, composições) que existem entre elas, modelando a estrutura estática da aplicação.

![Diagrama de Classe](ImagesPlantUML/classes.png)

---

### 🧩 Diagrama de Componentes

Demonstra como os componentes de software estão organizados e suas dependências mútuas, apresentando uma perspectiva modular da arquitetura e evidenciando como os diversos módulos lógicos se relacionam e trabalham em conjunto.

![Diagrama de Componentes](ImagesPlantUML/componentes.png)

---

### 💬 Diagramas de Comunicação

Os diagramas de comunicação exibem como objetos e componentes interagem em situações específicas, destacando a sequência de mensagens trocadas e a forma como os elementos colaboram para completar uma tarefa ou funcionalidade.

#### Diagrama de Comunicação: Cadastro de Aluno (UC-01)

Demonstra o fluxo de comunicação entre os componentes durante o processo de registro de um novo aluno.

![Diagrama de Comunicação: Cadastro de Aluno](ImagesPlantUML/comunicacao-cadastroaluno.png)

#### Diagrama de Comunicação: Visualizar Relatórios (UC-09/10)

Mostra como os componentes se comunicam para permitir que os usuários acessem e visualizem relatórios de progresso dos alunos e informações sobre as aulas realizadas.

![Diagrama de Comunicação: Visualizar Relatórios](ImagesPlantUML/comunicacao-visualizarrelatorios.png)

---

### 🔄 Diagramas de Estados

Modelam os diversos estados possíveis que entidades do sistema podem assumir durante seu ciclo de vida, além das condições e eventos que provocam mudanças de estado.

#### Diagrama de Estados: Status de Matrícula do Aluno

Modela o ciclo de vida da matrícula de um aluno, mostrando os possíveis estados (como `Pendente`, `Ativa`, `Suspensa`, `Cancelada`) e quais ações ou eventos causam a mudança entre esses estados.

![Diagrama de Estados: Status de Matrícula](ImagesPlantUML/estados-alunostatusmatricula.png)

#### Diagrama de Estados: Aula Prática

Descreve o ciclo de vida de uma aula prática, apresentando os estados possíveis (como `Agendada`, `Em Andamento`, `Concluída`, `Cancelada`) e os eventos que provocam as transições entre eles.

![Diagrama de Estados: Aula Prática](ImagesPlantUML/estados-aulapratica.png)

---

### 🚀 Diagrama de Implantação

Especifica a infraestrutura de hardware e a arquitetura de implantação em ambiente de nuvem, indicando os servidores necessários (como Servidor de Aplicação e Servidor de Arquivos) e quais componentes do software serão instalados em cada nó.

![Diagrama de Implantação](ImagesPlantUML/implantacao.png)

---

### 💾 Diagrama de Modelo de Dados

Apresenta o modelo entidade-relacionamento (ERD) do banco de dados, exibindo as tabelas, seus campos e os vínculos estabelecidos através de chaves primárias (`<PK>`) e estrangeiras (`<FK>`).

![Diagrama de Modelo de Dados](ImagesPlantUML/modelodedados.png)

---

### ⏳ Diagramas de Sequência

Os diagramas de sequência descrevem a ordem temporal das operações e a comunicação entre objetos ou atores durante a execução de uma funcionalidade, indicando o período de atividade de cada elemento envolvido no processo.

#### Diagrama de Sequência: Cadastrar Novo Aluno (UC-01)

Exibe a sequência temporal de operações e mensagens trocadas durante o processo de registro de um novo aluno.

![Diagrama de Sequência: Cadastrar Novo Aluno](ImagesPlantUML/sequencia-cadastrarnovoaluno.png)

#### Diagrama de Sequência: Marcar Presença (UC-06)

Demonstra a ordem das operações realizadas quando um instrutor ou funcionário registra a presença de um aluno em uma aula.

![Diagrama de Sequência: Marcar Presença](ImagesPlantUML/sequencia-marcarpresenca.png)

#### Diagrama de Sequência: Visualizar Relatório (UC-09/10)

Apresenta a sequência de chamadas e respostas necessárias para gerar e exibir relatórios de progresso dos alunos e de atividades das aulas.

![Diagrama de Sequência: Visualizar Relatório](ImagesPlantUML/sequencia-visualizarrelatorio.png)

#### Diagrama de Sequência: Agendar Aula Prática (UC-05)

Mostra o fluxo temporal de operações executadas quando um usuário agenda uma nova aula prática no sistema.

![Diagrama de Sequência: Agendar Aula Prática](ImagesPlantUML/sequencia2-agendaraulapratica.png)

#### Diagrama de Sequência: Cadastro de Funcionário (UC-02)

Descreve a ordem das interações e mensagens trocadas durante o processo de registro de um novo funcionário.

![Diagrama de Sequência: Cadastro de Funcionário](ImagesPlantUML/sequencia2-cadastrofuncionario.png)

#### Diagrama de Sequência: Visualizar Agenda (UC-07)

Exibe o fluxo de operações realizadas quando um usuário consulta a agenda de aulas disponível no sistema.

![Diagrama de Sequência: Visualizar Agenda](ImagesPlantUML/sequencia2-visualizaragenda.png)

---
