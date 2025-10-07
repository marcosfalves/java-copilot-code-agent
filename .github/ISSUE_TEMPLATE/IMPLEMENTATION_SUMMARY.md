# 📋 Issue Templates - Resumo da Implementação

## 🎯 Objetivo

Simplificar solicitações de mudança para professores através de formulários estruturados de issue templates que fornecem detalhes suficientes para o agente de codificação Copilot realizar as tarefas sem explicações adicionais.

## 📦 O Que Foi Criado

### 7 Templates de Issue (em formato YAML)

1. **🎓 Adicionar Nova Atividade** (`add-new-activity.yml`)
   - Para solicitar adição de novas atividades extracurriculares
   - Captura: nome, descrição, categoria, horários, capacidade, professor responsável
   - Inclui validações e orientações técnicas de implementação

2. **✏️ Modificar Atividade Existente** (`modify-activity.yml`)
   - Para alterar atividades já cadastradas
   - Permite modificação seletiva de campos específicos
   - Inclui justificativa e validações (ex: capacidade vs inscritos atuais)

3. **🐛 Reportar Bug** (`bug-report.yml`)
   - Para reportar problemas e erros no sistema
   - Captura: área afetada, passos para reproduzir, comportamento esperado vs atual
   - Inclui campos para mensagens de erro e frequência do problema

4. **✨ Solicitar Nova Funcionalidade** (`feature-request.yml`)
   - Para sugerir novas funcionalidades ou melhorias
   - Captura: descrição, problema que resolve, solução proposta, história de usuário
   - Inclui prioridade, usuários afetados, critérios de aceitação

5. **👥 Gerenciar Inscrição de Estudante** (`student-enrollment.yml`)
   - Para resolver problemas com inscrições de estudantes
   - Captura: tipo de solicitação, atividade, email do estudante, situação atual
   - Inclui urgência, justificativa, e múltiplos cenários (inscrever, cancelar, transferir)

6. **🎨 Melhorar Interface do Usuário** (`ui-improvement.yml`)
   - Para solicitar melhorias visuais ou de usabilidade
   - Captura: área da interface, tipo de melhoria, estado atual vs proposto
   - Inclui aspectos de design (acessibilidade, responsividade, performance)

7. **⚙️ Configuração** (`config.yml`)
   - Configuração dos templates com links úteis
   - Referências para documentação, discussões e ajuda urgente
   - Permite criação de issues em branco quando necessário

8. **📚 Guia de Uso** (`README.md`)
   - Documentação completa sobre qual template usar
   - Exemplos de uso para cada template
   - Dicas de boas práticas
   - Explicação de como o Copilot usa os templates

## ✨ Características Principais

### Para os Professores
- ✅ **Formulários estruturados** - Campos claros e objetivos
- ✅ **Exemplos em português** - Todos os textos em PT-BR
- ✅ **Validações** - Campos obrigatórios claramente marcados
- ✅ **Opções de seleção** - Dropdowns e checkboxes para facilitar preenchimento
- ✅ **Placeholders úteis** - Exemplos em cada campo
- ✅ **Guia de uso** - README explicando qual template usar

### Para o Agente Copilot
- 🤖 **Critérios de aceitação claros** - Em cada template
- 🤖 **Contexto técnico detalhado** - Arquivos a modificar, padrões a seguir
- 🤖 **Exemplos de código** - Snippets mostrando como implementar
- 🤖 **Validações especificadas** - Regras de negócio documentadas
- 🤖 **Arquitetura considerada** - Orientações seguindo Clean Architecture

## 📊 Estrutura dos Templates

Cada template segue um padrão consistente:

```yaml
name: [Nome do Template]
description: [Descrição breve]
title: "[TAG] "
labels: ["label1", "label2"]
body:
  - Markdown de introdução
  - Campos de entrada (input, textarea, dropdown, checkboxes)
  - Seção de Critérios de Aceitação
  - Seção de Contexto Técnico para o Agente
```

### Tipos de Campos Usados

- **input**: Para dados de uma linha (nome, horário, capacidade)
- **textarea**: Para descrições longas e múltiplas linhas
- **dropdown**: Para seleção única entre opções predefinidas
- **checkboxes**: Para seleção múltipla (dias da semana, campos a modificar)
- **markdown**: Para instruções, exemplos e contexto técnico

## 🎓 Alinhamento com Requisitos

### Descrição Clara do Problema ✅
- Cada template tem campos específicos para descrever o problema/necessidade
- Exemplos e placeholders ajudam a clarificar expectativas
- Campos de "situação atual" vs "resultado desejado"

### Critérios de Aceitação Claros ✅
- Seção dedicada em todos os templates
- Checklist de itens que devem ser cumpridos
- Validações técnicas especificadas

### Dicas e Soluções para Começar ✅
- Seção "Contexto Técnico para o Agente" em todos os templates
- Exemplos de código para implementação
- Referências a arquivos relevantes do projeto
- Padrões e convenções a seguir

### Limitações e Contexto ✅
- Validações de negócio documentadas
- Considerações de arquitetura incluídas
- Impactos em outras partes do sistema mencionados
- Links para documentação adicional

## 🔧 Detalhes Técnicos

### Localização
```
.github/
└── ISSUE_TEMPLATE/
    ├── README.md                    # Guia de uso
    ├── config.yml                   # Configuração
    ├── add-new-activity.yml         # Template 1
    ├── modify-activity.yml          # Template 2
    ├── bug-report.yml               # Template 3
    ├── feature-request.yml          # Template 4
    ├── student-enrollment.yml       # Template 5
    └── ui-improvement.yml           # Template 6
```

### Validação
- ✅ Todos os arquivos YAML validados sintaticamente
- ✅ Campos obrigatórios marcados com `required: true`
- ✅ Estrutura consistente entre templates
- ✅ Textos em português brasileiro

### Integração com GitHub
- Templates aparecem automaticamente ao criar nova issue
- Seletor visual mostra todos os templates disponíveis
- Formulários são renderizados como interface web amigável
- Issues criadas já vêm com labels apropriados
- Títulos pré-formatados com tags ([ATIVIDADE], [BUG], etc.)

## 📈 Benefícios Esperados

### Para Professores
1. **Redução de barreiras** - Não precisam saber programação
2. **Clareza no processo** - Sabem exatamente o que fornecer
3. **Menos idas e vindas** - Informações completas desde o início
4. **Confiança aumentada** - Templates guiam o processo

### Para o Agente Copilot
1. **Informações completas** - Todos os dados necessários desde o início
2. **Contexto técnico** - Sabe exatamente onde e como implementar
3. **Validações claras** - Regras de negócio bem definidas
4. **Padrões estabelecidos** - Exemplos de código a seguir

### Para o Projeto
1. **Issues bem formadas** - Informações estruturadas e completas
2. **Menos retrabalho** - Requisitos claros desde o início
3. **Histórico organizado** - Labels e títulos consistentes
4. **Rastreabilidade** - Fácil encontrar issues por tipo

## 🚀 Como Usar

### Para Professores
1. Ir para a aba "Issues" no GitHub
2. Clicar em "New Issue"
3. Escolher o template apropriado
4. Preencher os campos do formulário
5. Submeter a issue

### Para o Agente Copilot
1. Ler os campos preenchidos pelo professor
2. Consultar a seção "Contexto Técnico para o Agente"
3. Seguir os exemplos de código fornecidos
4. Implementar respeitando a arquitetura do projeto
5. Validar contra os critérios de aceitação

## 📝 Exemplos de Issues Geradas

### Exemplo 1: Adicionar Nova Atividade
```
Título: [ATIVIDADE] Clube de Robótica
Labels: enhancement, activity

Nome da Atividade: Clube de Robótica
Descrição: Os alunos aprenderão fundamentos...
Categoria: Tecnologia
Dias da Semana: ✓ Segunda-feira, ✓ Quarta-feira
Horário de Início: 15:30
Horário de Término: 17:00
Capacidade Máxima: 15
Professor Responsável: Prof. Chen
```

### Exemplo 2: Reportar Bug
```
Título: [BUG] Inscrição não funciona apesar de haver vagas
Labels: bug

Área do Sistema: Inscrição de Estudantes
Descrição: Quando tento inscrever um estudante...
Passos para Reproduzir:
1. Fazer login como professor
2. Clicar em "Inscrever-se" no Chess Club
...
Frequência: Sempre (100% das vezes)
```

## 🎯 Próximos Passos

1. ✅ Templates criados e validados
2. ⏳ Templates serão visíveis após merge no GitHub
3. ⏳ Professores podem começar a usar
4. ⏳ Coletar feedback e iterar conforme necessário
5. ⏳ Adicionar mais templates se novos padrões emergirem

## 📚 Referências

- [GitHub Issue Forms Documentation](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms)
- [GitHub Issue Templates Best Practices](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository)
- Documentação do Sistema: `docs/README.md`

---

**Data de Criação:** Outubro 2024  
**Autor:** GitHub Copilot Agent  
**Status:** ✅ Completo e Pronto para Uso
