# 🧩 Ciclo Completo de Construção de um Sistema

Este documento apresenta as principais etapas envolvidas na construção de um sistema de software, desde a concepção da ideia até sua manutenção e evolução.

O objetivo é utilizar esse ciclo como referência para um projeto inicial de programação, permitindo contato com diferentes áreas e etapas do desenvolvimento de software.

---

# 📋 Índice

1. [Ideia](#1--ideia)
2. [Levantamento de Requisitos](#2--levantamento-de-requisitos)
3. [Análise do Sistema](#3--análise-do-sistema)
4. [Planejamento](#4--planejamento)
5. [Modelagem](#5--modelagem)
6. [UX/UI e Prototipação](#6--uxui-e-prototipação)
7. [Arquitetura do Sistema](#7--arquitetura-do-sistema)
8. [Desenvolvimento](#8--desenvolvimento)
9. [Testes](#9--testes)
10. [Implantação](#10--implantação)
11. [Documentação](#11--documentação)
12. [Manutenção e Evolução](#12--manutenção-e-evolução)
13. [Controle de Versão](#13--controle-de-versão)
14. [Ciclo de Vida](#14--ciclo-de-vida)
15. [Resumo das Etapas](#15--resumo-das-etapas)

---

# 1. 💡 Ideia

A ideia representa o nascimento do projeto.
É o momento em que uma necessidade ou problema é identificado e transformado em uma ideia de sistema.

## Atividades

* Identificar um problema / necessidade
* Definir a ideia do sistema
* Identificar quem utilizará o sistema
* Definir o objetivo principal
* Definir o que o sistema deverá resolver
* Definir o que não faz parte do projeto
* Identificar possíveis soluções
* Definir uma visão inicial do produto

## Documentos possíveis

* Descrição da ideia
* Visão do projeto
* Objetivos
* Público-alvo
* Escopo inicial

---

# 2. 📝 Levantamento de Requisitos

Nesta etapa, a ideia começa a ser transformada em especificações que possam ser compreendidas e posteriormente implementadas.

## 2.1 Requisitos Funcionais

Definem **o que o sistema deve fazer**.

Exemplos:

* Cadastrar usuário
* Fazer login
* Criar comunicado
* Editar comunicado
* Excluir comunicado
* Pesquisar comunicado
* Enviar notificações

## 2.2 Requisitos Não Funcionais

Definem **como o sistema deve funcionar**.

Exemplos:

* Segurança
* Desempenho
* Disponibilidade
* Compatibilidade
* Acessibilidade
* Responsividade
* Usabilidade
* Privacidade

## 2.3 Regras de Negócio

Definem as regras específicas que o sistema deverá seguir.

Exemplo:

> Apenas administradores podem excluir comunicados.

## 2.4 Perfis de Usuário

Identificar os diferentes tipos de usuários que utilizarão o sistema.

Exemplos:

* Administrador
* Usuário comum
* Moderador
* Visitante
* Outros perfis específicos do projeto

## Documentos

* Lista de requisitos
* Requisitos funcionais
* Requisitos não funcionais
* Regras de negócio
* Casos de uso
* Histórias de usuário

---

# 3. 🔎 Análise do Sistema

Nesta etapa, os requisitos são analisados para determinar como o sistema deverá funcionar.

## Atividades

* Analisar os requisitos
* Identificar entidades
* Identificar processos
* Identificar entradas
* Identificar saídas
* Identificar dependências
* Identificar riscos
* Identificar integrações externas
* Identificar permissões
* Identificar possíveis problemas

## Modelos possíveis

* Diagrama de casos de uso
* Fluxogramas
* Diagramas de atividades
* Diagramas de sequência
* Mapas de processos

---

# 4. 📅 Planejamento

O planejamento define como o projeto será desenvolvido.

## Atividades

* Definir tecnologias
* Definir linguagem de programação
* Definir banco de dados
* Definir ferramentas
* Dividir o projeto em tarefas
* Definir prioridades
* Definir versões
* Definir milestones
* Estimar esforço
* Definir cronograma
* Definir responsáveis
* Identificar riscos

## Exemplos de ferramentas

* Git
* GitHub
* Visual Studio Code
* Figma
* Trello
* Jira
* Docker

---

# 5. 🗄️ Modelagem

A modelagem define a estrutura interna do sistema.

---

## 5.1 Modelagem de Dados

Definir:

* Entidades
* Atributos
* Relacionamentos
* Chaves primárias
* Chaves estrangeiras
* Restrições
* Índices

### Exemplo

```text
USUÁRIO
 ├── id
 ├── nome
 ├── email
 └── senha

COMUNICADO
 ├── id
 ├── título
 ├── conteúdo
 ├── data
 └── usuário_id
```

---

## 5.2 Banco de Dados

Definir:

* Modelo conceitual
* Modelo lógico
* Modelo físico
* Tabelas
* Relacionamentos
* Queries
* Views
* Procedures, quando aplicável

---

# 6. 🎨 UX/UI e Prototipação

Antes de programar a interface, podemos projetá-la.

---

## 6.1 UX — User Experience

A UX trata da experiência do usuário ao utilizar o sistema.

### Definições

* Jornada do usuário
* Navegação
* Fluxos
* Usabilidade
* Acessibilidade
* Organização das informações

---

## 6.2 UI — User Interface

A UI trata dos elementos visuais da interface.

### Definições

* Cores
* Tipografia
* Botões
* Menus
* Ícones
* Cards
* Formulários
* Layout
* Responsividade

---

## 6.3 Prototipação

Criar:

* Wireframes
* Mockups
* Protótipo navegável

### Ferramenta

* Figma

---

# 7. 🏗️ Arquitetura do Sistema

A arquitetura define como as diferentes partes do sistema serão organizadas e como elas irão se comunicar.

## Exemplo

```text
                 SISTEMA
                    │
        ┌───────────┼───────────┐
        │           │           │
     FRONTEND     BACKEND    BANCO
        │           │           │
        │       API/REST       │
        │           │           │
        └───────────┴───────────┘
```

## Definições

* Arquitetura
* Camadas
* APIs
* Comunicação entre componentes
* Autenticação
* Autorização
* Banco de dados
* Serviços externos
* Estrutura de pastas
* Padrões de projeto

## Exemplos de arquiteturas

* MVC
* REST
* Cliente/Servidor
* Monolito
* Microsserviços

> Para um primeiro projeto, normalmente não é necessário começar com uma arquitetura de microsserviços.

---

# 8. 👨‍💻 Desenvolvimento

Nesta etapa ocorre a implementação do sistema.

---

## 8.1 Configuração do Ambiente

* Instalar ferramentas
* Configurar IDE
* Configurar Git
* Criar repositório
* Configurar banco de dados
* Criar estrutura inicial do projeto

---

## 8.2 Desenvolvimento do Frontend

Possíveis tecnologias:

* HTML
* CSS
* JavaScript
* Frameworks
* Bibliotecas

### Atividades

* Criar páginas
* Criar componentes
* Criar formulários
* Implementar validações
* Implementar navegação
* Implementar responsividade

---

## 8.3 Desenvolvimento do Backend

### Atividades

* Criar servidor
* Criar rotas
* Criar controllers
* Criar services
* Implementar regras de negócio
* Criar APIs
* Implementar autenticação
* Implementar autorização

---

## 8.4 Desenvolvimento do Banco

### Atividades

* Criar tabelas
* Criar relacionamentos
* Inserir dados
* Consultar dados
* Atualizar dados
* Excluir dados

---

## 8.5 Integração

Conectar as diferentes partes do sistema.

```text
Frontend
    ↓
API
    ↓
Backend
    ↓
Banco de Dados
```

---

# 9. 🧪 Testes

Os testes verificam se o sistema funciona corretamente e se atende aos requisitos definidos.

---

## 9.1 Testes Unitários

Testam pequenas partes do código isoladamente.

Exemplo:

```text
função calcularTotal()
       ↓
     TESTE
       ↓
   resultado
```

---

## 9.2 Testes de Integração

Verificam se diferentes componentes funcionam corretamente em conjunto.

Exemplo:

```text
Frontend → API → Banco
```

---

## 9.3 Testes Funcionais

Verificam se as funcionalidades funcionam de acordo com os requisitos.

Exemplo:

```text
Requisito:
"Usuário deve conseguir realizar login."

        ↓

Teste:
Informar usuário + senha
        ↓
Sistema autentica
        ↓
Usuário acessa o sistema
```

---

## 9.4 Testes de Interface

Verificar:

* Botões
* Formulários
* Menus
* Navegação
* Responsividade
* Layout

---

## 9.5 Testes de Segurança

Verificar:

* Login
* Permissões
* Senhas
* Sessões
* Entrada de dados
* SQL Injection
* XSS
* Controle de acesso

---

## 9.6 Testes de Desempenho

Verificar:

* Tempo de resposta
* Carga
* Quantidade de usuários
* Consumo de recursos
* Capacidade do sistema

---

## 9.7 Testes de Aceitação

Verificar se o sistema atende às necessidades para as quais foi desenvolvido.

---

# 10. 🚀 Implantação

Nesta etapa o sistema deixa o ambiente de desenvolvimento e passa a funcionar em um ambiente real.

## Ambientes

```text
DESENVOLVIMENTO
       ↓
     TESTES
       ↓
   HOMOLOGAÇÃO
       ↓
    PRODUÇÃO
```

## Atividades

* Configurar servidor
* Configurar banco de dados
* Configurar domínio
* Configurar HTTPS
* Configurar variáveis de ambiente
* Fazer build
* Publicar aplicação
* Configurar backups
* Configurar logs

---

# 11. 📚 Documentação

A documentação registra como o sistema funciona, como foi desenvolvido e como deve ser utilizado.

A documentação deve acompanhar o projeto durante todo o desenvolvimento.

---

## 11.1 Documentação Técnica

* Arquitetura
* Banco de dados
* APIs
* Estrutura do projeto
* Instalação
* Configuração
* Dependências

---

## 11.2 Documentação do Usuário

* Manual
* FAQ
* Tutoriais
* Procedimentos

---

## 11.3 Documentação do Código

* Comentários relevantes
* JSDoc
* Docstrings
* Convenções de código

---

## 11.4 Documentação do Projeto

* Requisitos
* Decisões técnicas
* Versões
* Alterações
* Histórico

---

# 12. 🔧 Manutenção e Evolução

O desenvolvimento não termina quando o sistema é publicado.

Após a implantação começam novas atividades.

---

## 12.1 Correção

* Correção de bugs
* Correção de erros
* Correções de segurança

---

## 12.2 Manutenção

* Atualização de dependências
* Atualização do servidor
* Atualização do banco de dados
* Melhorias de desempenho

---

## 12.3 Evolução

* Novas funcionalidades
* Novas telas
* Novas integrações
* Melhorias de UX
* Melhorias de desempenho

---

## 12.4 Monitoramento

Monitorar:

* Logs
* Erros
* Desempenho
* Disponibilidade
* Uso do sistema

---

# 13. 🔄 Controle de Versão

O controle de versão deve acompanhar praticamente todo o projeto.

Uma ferramenta muito utilizada é o **Git**.

## Exemplo de versões

```text
Projeto
│
├── v0.1
├── v0.2
├── v0.3
├── v1.0
├── v1.1
└── v2.0
```

## Fluxo básico

```text
Código
  ↓
Git
  ↓
Commit
  ↓
Branch
  ↓
Pull Request
  ↓
Merge
  ↓
Release
```

O controle de versão permite:

* Registrar alterações
* Recuperar versões anteriores
* Trabalhar com branches
* Trabalhar em equipe
* Revisar código
* Criar releases
* Manter histórico do projeto

---

# 14. 🔁 Ciclo de Vida

O desenvolvimento de software não deve ser encarado como uma sequência completamente linear.

Na prática, o processo é cíclico.

```text
                 ┌──────────────┐
                 │    IDEIA     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │  REQUISITOS  │
                 └──────┬───────┘
                        ↓
                  ┌───────────┐
                  │  ANÁLISE  │
                  └─────┬─────┘
                        ↓
                 ┌──────────────┐
                 │  PROJETO     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │ DESENVOLV.   │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │    TESTES    │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │   DEPLOY     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │   USO REAL   │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │  FEEDBACK    │
                 └──────┬───────┘
                        │
                        └──────────→ REQUISITOS
```

O feedback dos usuários pode gerar novos requisitos, iniciando um novo ciclo de desenvolvimento.

---

# 15. 📊 Resumo das Etapas

|  # | Etapa             | Principal aprendizado                 |
| -: | ----------------- | ------------------------------------- |
| 01 | Ideia             | Identificação do problema             |
| 02 | Escopo            | Definição dos limites                 |
| 03 | Requisitos        | O que o sistema precisa fazer         |
| 04 | Regras de negócio | Como o sistema deve funcionar         |
| 05 | Análise           | Transformar necessidades em processos |
| 06 | Planejamento      | Organizar o desenvolvimento           |
| 07 | UX                | Pensar na experiência do usuário      |
| 08 | UI                | Projetar a interface                  |
| 09 | Modelagem         | Estruturar informações e processos    |
| 10 | Banco de dados    | Persistência dos dados                |
| 11 | Arquitetura       | Organizar tecnicamente o sistema      |
| 12 | Ambiente          | Preparar as ferramentas               |
| 13 | Git               | Controle de versão                    |
| 14 | Frontend          | Construir a interface                 |
| 15 | Backend           | Construir a lógica                    |
| 16 | API               | Comunicação entre sistemas            |
| 17 | Integração        | Unir todas as partes                  |
| 18 | Testes            | Verificar funcionamento               |
| 19 | Segurança         | Proteger sistema e dados              |
| 20 | Homologação       | Validar o produto                     |
| 21 | Deploy            | Publicar                              |
| 22 | Documentação      | Registrar conhecimento                |
| 23 | Monitoramento     | Acompanhar o sistema                  |
| 24 | Manutenção        | Corrigir problemas                    |
| 25 | Evolução          | Criar novas versões                   |

---

# 🏁 Conclusão

Um projeto inicial de programação pode ser utilizado para aprender muito mais do que apenas uma linguagem de programação.

Ao percorrer todas essas etapas, é possível ter contato com:

```text
                    SOFTWARE
                       │
       ┌───────────────┼────────────────┐
       │               │                │
    NEGÓCIO          DESIGN          TECNOLOGIA
       │               │                │
  Requisitos          UX             Frontend
  Processos           UI             Backend
  Regras              UX             Banco
  Escopo              Protótipo      APIs
       │               │                │
       └───────────────┼────────────────┘
                       │
                  DESENVOLVIMENTO
                       │
              ┌────────┴────────┐
              │                 │
            TESTES          VERSIONAMENTO
              │                 │
              └────────┬────────┘
                       │
                    DEPLOY
                       │
                  PRODUÇÃO
                       │
                 MONITORAMENTO
                       │
                 MANUTENÇÃO
                       │
                    EVOLUÇÃO
                       │
                       └──────→ NOVO CICLO
```

Dessa forma, o projeto passa a funcionar como uma **experiência prática do ciclo de vida completo de um sistema**, permitindo estudar programação dentro de um contexto real de desenvolvimento de software.
