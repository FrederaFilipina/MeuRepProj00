# Ciclo Completo de Construção de um Sistema

## Visão geral

Se a ideia é que um primeiro projeto de programação sirva como uma experiência completa de desenvolvimento de software, o projeto pode passar por praticamente todo o ciclo de vida de um sistema — desde a ideia inicial até a manutenção e evolução.

```text
1. IDEIA
   ↓
2. LEVANTAMENTO DE REQUISITOS
   ↓
3. ANÁLISE
   ↓
4. PLANEJAMENTO
   ↓
5. MODELAGEM
   ↓
6. UX/UI E PROTOTIPAÇÃO
   ↓
7. ARQUITETURA
   ↓
8. DESENVOLVIMENTO
   ↓
9. TESTES
   ↓
10. IMPLANTAÇÃO
   ↓
11. DOCUMENTAÇÃO
   ↓
12. MANUTENÇÃO E EVOLUÇÃO
```

---

# 1. 💡 Ideação

É o nascimento do projeto.

## Atividades

- Identificar um problema
- Identificar uma necessidade
- Definir a ideia do sistema
- Identificar quem utilizará o sistema
- Definir o objetivo principal
- Definir o que o sistema deverá resolver
- Definir o que **não** faz parte do projeto
- Identificar possíveis soluções
- Definir uma visão inicial do produto

## Documentos possíveis

- Descrição da ideia
- Visão do projeto
- Objetivos
- Público-alvo
- Escopo inicial

---

# 2. 📝 Levantamento de Requisitos

Aqui começamos a transformar a ideia em algo que possa ser desenvolvido.

## 2.1 Requisitos funcionais

Definem **o que o sistema faz**.

Exemplos:

- Cadastrar usuário
- Fazer login
- Criar comunicado
- Editar comunicado
- Excluir comunicado
- Pesquisar comunicado
- Enviar notificações

## 2.2 Requisitos não funcionais

Definem **como o sistema deve funcionar**.

Exemplos:

- Segurança
- Desempenho
- Disponibilidade
- Compatibilidade
- Acessibilidade
- Responsividade
- Usabilidade
- Privacidade

## 2.3 Regras de negócio

Definem as regras específicas do sistema.

Exemplo:

> Apenas administradores podem excluir comunicados.

## 2.4 Levantamento dos usuários

Identificar:

- Administrador
- Usuário comum
- Moderador
- Visitante
- Outros perfis

## Documentos

- Lista de requisitos
- Requisitos funcionais
- Requisitos não funcionais
- Regras de negócio
- Casos de uso
- Histórias de usuário

---

# 3. 🔎 Análise do Sistema

Agora analisamos os requisitos para descobrir **como o sistema deverá funcionar**.

## Atividades

- Analisar os requisitos
- Identificar entidades
- Identificar processos
- Identificar entradas
- Identificar saídas
- Identificar dependências
- Identificar riscos
- Identificar integrações externas
- Identificar permissões
- Identificar possíveis problemas

## Modelos possíveis

- Diagrama de casos de uso
- Fluxogramas
- Diagramas de atividades
- Diagramas de sequência
- Mapas de processos

---

# 4. 📅 Planejamento

Agora definimos **como o projeto será desenvolvido**.

## Atividades

- Definir tecnologias
- Definir linguagem de programação
- Definir banco de dados
- Definir ferramentas
- Dividir o projeto em tarefas
- Definir prioridades
- Definir versões
- Definir milestones
- Estimar esforço
- Definir cronograma
- Definir responsáveis
- Identificar riscos

## Exemplos de ferramentas

- Git
- GitHub
- VS Code
- Figma
- Trello
- Jira
- Docker

---

# 5. 🗄️ Modelagem

Aqui começamos a construir a estrutura interna do sistema.

## 5.1 Modelagem de dados

Definir:

- Entidades
- Atributos
- Relacionamentos
- Chaves primárias
- Chaves estrangeiras
- Restrições
- Índices

Exemplo:

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

## 5.2 Banco de dados

Definir:

- Modelo conceitual
- Modelo lógico
- Modelo físico
- Tabelas
- Relacionamentos
- Queries
- Views
- Procedures, quando aplicável

---

# 6. 🎨 UX/UI e Prototipação

Antes de programar a interface, podemos desenhá-la.

## UX

Pensar em:

- Jornada do usuário
- Navegação
- Fluxos
- Usabilidade
- Acessibilidade

## UI

Definir:

- Cores
- Tipografia
- Botões
- Menus
- Ícones
- Cards
- Formulários
- Layout
- Responsividade

## Prototipação

Criar:

- Wireframes
- Mockups
- Protótipo navegável

### Ferramenta bastante utilizada

- Figma

---

# 7. 🏗️ Arquitetura do Sistema

Aqui decidimos **como as partes do sistema serão organizadas**.

Exemplo:

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

- Arquitetura
- Camadas
- APIs
- Comunicação entre componentes
- Autenticação
- Autorização
- Banco de dados
- Serviços externos
- Estrutura de pastas
- Padrões de projeto

## Exemplos

- MVC
- REST
- Cliente/Servidor
- Monolito
- Microsserviços

> Para um primeiro projeto, normalmente não há necessidade de começar com microsserviços.

---

# 8. 👨‍💻 Desenvolvimento

Finalmente começa a implementação.

## 8.1 Configuração do ambiente

- Instalar ferramentas
- Configurar IDE
- Configurar Git
- Criar repositório
- Configurar banco
- Criar estrutura inicial

## 8.2 Desenvolvimento do frontend

- HTML
- CSS
- JavaScript
- Framework, se necessário
- Componentes
- Formulários
- Validações
- Responsividade

## 8.3 Desenvolvimento do backend

- Servidor
- Rotas
- Controllers
- Services
- Regras de negócio
- APIs
- Autenticação
- Autorização

## 8.4 Banco de dados

- Criar tabelas
- Criar relacionamentos
- Inserir dados
- Consultar dados
- Atualizar dados
- Excluir dados

## 8.5 Integração

Conectar:

```text
Frontend
    ↓
API
    ↓
Backend
    ↓
Banco de dados
```

---

# 9. 🧪 Testes

Uma das etapas mais importantes.

## 9.1 Testes unitários

Testar pequenas partes do código.

```text
função calcularTotal()
       ↓
     TESTE
       ↓
   resultado
```

## 9.2 Testes de integração

Verificar se diferentes componentes funcionam juntos.

Exemplo:

```text
Frontend → API → Banco
```

## 9.3 Testes funcionais

Verificar se uma funcionalidade funciona conforme o requisito.

## 9.4 Testes de interface

Verificar:

- Botões
- Formulários
- Navegação
- Responsividade

## 9.5 Testes de segurança

Verificar:

- Login
- Permissões
- Senhas
- Sessões
- Entrada de dados
- SQL Injection
- XSS

## 9.6 Testes de desempenho

Verificar:

- Tempo de resposta
- Carga
- Quantidade de usuários
- Consumo de recursos

## 9.7 Teste de aceitação

Verificar se o sistema realmente atende ao que foi solicitado.

---

# 10. 🚀 Implantação

O sistema deixa o ambiente de desenvolvimento e passa a funcionar em um ambiente real.

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

- Configurar servidor
- Configurar banco
- Configurar domínio
- Configurar HTTPS
- Configurar variáveis de ambiente
- Fazer build
- Publicar aplicação
- Configurar backups
- Configurar logs

---

# 11. 📚 Documentação

A documentação deve acompanhar o projeto, não ser deixada apenas para o final.

## 11.1 Documentação técnica

- Arquitetura
- Banco de dados
- APIs
- Estrutura do projeto
- Instalação
- Configuração
- Dependências

## 11.2 Documentação do usuário

- Manual
- FAQ
- Tutoriais
- Procedimentos

## 11.3 Documentação do código

- Comentários relevantes
- JSDoc
- Docstrings
- Convenções

## 11.4 Documentação do projeto

- Requisitos
- Decisões
- Versões
- Alterações
- Histórico

---

# 12. 🔧 Manutenção e Evolução

O desenvolvimento **não termina quando o sistema é publicado**.

Depois da implantação começam outras atividades.

## 12.1 Correção

- Bugs
- Erros
- Problemas de segurança

## 12.2 Manutenção

- Atualização de dependências
- Atualização do servidor
- Atualização do banco
- Melhorias de desempenho

## 12.3 Evolução

- Novas funcionalidades
- Novas telas
- Novas integrações
- Melhorias de UX

## 12.4 Monitoramento

- Logs
- Erros
- Desempenho
- Disponibilidade
- Uso do sistema

---

# 13. 🔄 Controle de Versão

O controle de versão é uma atividade transversal que acompanha **todo o projeto**.

Uma ferramenta comum é o Git.

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

Isso permite trabalhar com histórico, versões, branches, colaboração e recuperação de alterações.

---

# 📋 Resumo das Etapas

| # | Etapa | Principal aprendizado |
|---:|---|---|
| 01 | Ideia | Identificação do problema |
| 02 | Escopo | Definição dos limites |
| 03 | Requisitos | O que o sistema precisa fazer |
| 04 | Regras de negócio | Como o sistema deve funcionar |
| 05 | Análise | Transformar necessidades em processos |
| 06 | Planejamento | Organizar o desenvolvimento |
| 07 | UX | Pensar na experiência do usuário |
| 08 | UI | Projetar a interface |
| 09 | Modelagem | Estruturar informações e processos |
| 10 | Banco de dados | Persistência dos dados |
| 11 | Arquitetura | Organizar tecnicamente o sistema |
| 12 | Ambiente | Preparar ferramentas |
| 13 | Git | Controle de versão |
| 14 | Frontend | Construir a interface |
| 15 | Backend | Construir a lógica |
| 16 | API | Comunicação entre sistemas |
| 17 | Integração | Unir todas as partes |
| 18 | Testes | Verificar funcionamento |
| 19 | Segurança | Proteger sistema e dados |
| 20 | Homologação | Validar o produto |
| 21 | Deploy | Publicar |
| 22 | Documentação | Registrar conhecimento |
| 23 | Monitoramento | Acompanhar o sistema |
| 24 | Manutenção | Corrigir problemas |
| 25 | Evolução | Criar novas versões |

---

# 🔁 O ciclo não é linear

O desenvolvimento de software não precisa seguir uma linha reta. O feedback obtido durante o uso pode gerar novos requisitos e iniciar um novo ciclo.

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
                        └──────────────→ REQUISITOS
```

---

# 🎓 Estrutura Recomendada para um Primeiro Projeto

Se o objetivo é **aprender programação através da construção de um sistema completo**, uma sequência didática possível é:

1. Ideia
2. Escopo
3. Requisitos
4. Regras de negócio
5. Análise
6. Planejamento
7. UX
8. UI
9. Modelagem
10. Banco de dados
11. Arquitetura
12. Configuração do ambiente
13. Git
14. Frontend
15. Backend
16. API
17. Integração
18. Testes
19. Segurança
20. Homologação
21. Deploy
22. Documentação
23. Monitoramento
24. Manutenção
25. Evolução

Dessa forma, o projeto deixa de ser apenas um exercício de programação e passa a funcionar como uma **experiência prática do ciclo de desenvolvimento de software**, envolvendo análise, documentação, banco de dados, interface, programação, testes, versionamento, segurança, publicação e manutenção.
