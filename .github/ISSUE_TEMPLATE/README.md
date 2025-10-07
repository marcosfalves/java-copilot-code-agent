# 📝 Guia de Templates de Issue

Este diretório contém templates de issue que facilitam a solicitação de mudanças no sistema de gestão escolar.

## 🎯 Qual Template Usar?

### 🎓 [Adicionar Nova Atividade](add-new-activity.yml)
**Use quando:** Você quer adicionar uma nova atividade extracurricular ao sistema.

**Exemplos:**
- Criar um novo "Clube de Robótica"
- Adicionar "Aulas de Piano"
- Criar "Time de Vôlei"

**O que é solicitado:**
- Nome, descrição e categoria da atividade
- Dias da semana e horários
- Capacidade máxima e professor responsável

---

### ✏️ [Modificar Atividade Existente](modify-activity.yml)
**Use quando:** Você precisa alterar informações de uma atividade já cadastrada.

**Exemplos:**
- Mudar horário do Chess Club
- Aumentar capacidade do Art Club
- Alterar descrição do Drama Club
- Trocar os dias de uma atividade

**O que é solicitado:**
- Nome da atividade a modificar
- Quais campos devem ser alterados
- Novos valores e justificativa

---

### 🐛 [Reportar Bug](bug-report.yml)
**Use quando:** Algo não está funcionando corretamente no sistema.

**Exemplos:**
- Não consigo inscrever um estudante mesmo havendo vagas
- Login não funciona
- Filtro de busca retorna resultados errados
- Erro ao cancelar inscrição

**O que é solicitado:**
- Descrição do problema
- Passos para reproduzir
- Comportamento esperado vs. atual
- Mensagens de erro

---

### ✨ [Solicitar Nova Funcionalidade](feature-request.yml)
**Use quando:** Você tem uma ideia para melhorar o sistema com algo novo.

**Exemplos:**
- Exportar lista de participantes para Excel
- Enviar emails automáticos de confirmação
- Adicionar campo de observações nas atividades
- Criar relatórios de frequência

**O que é solicitado:**
- Descrição da funcionalidade
- Problema que resolve
- Como deveria funcionar
- Quem se beneficiaria

---

### 👥 [Gerenciar Inscrição de Estudante](student-enrollment.yml)
**Use quando:** Você precisa resolver problemas ou fazer mudanças em inscrições.

**Exemplos:**
- Inscrever estudante quando sistema não permite
- Cancelar inscrição de estudante
- Transferir estudante entre atividades
- Aumentar capacidade temporariamente

**O que é solicitado:**
- Tipo de solicitação
- Nome da atividade e email do estudante
- Situação atual e resultado desejado
- Justificativa e urgência

---

### 🎨 [Melhorar Interface do Usuário](ui-improvement.yml)
**Use quando:** Você quer melhorar o visual ou usabilidade da interface web.

**Exemplos:**
- Mudar cores do site
- Melhorar layout dos cartões
- Adicionar ícones
- Corrigir problemas de visualização mobile
- Melhorar acessibilidade

**O que é solicitado:**
- Área e tipo de melhoria
- Estado atual vs. proposta
- Benefício para usuários
- Referências visuais (opcional)

---

## 💡 Dicas para Criar Issues Efetivas

### ✅ Faça:
- **Seja específico:** Quanto mais detalhes, melhor o agente Copilot pode ajudar
- **Use exemplos:** Exemplos concretos são mais claros que descrições abstratas
- **Preencha todos os campos obrigatórios:** Campos marcados com * são essenciais
- **Inclua contexto:** Explique por que a mudança é necessária
- **Forneça dados reais:** Use nomes reais de atividades, emails válidos, etc.

### ❌ Evite:
- Descrições vagas como "melhorar o sistema"
- Misturar múltiplas solicitações em uma issue
- Deixar campos obrigatórios vazios
- Usar termos técnicos desnecessários

---

## 🤖 Como o Agente Copilot Usa Estes Templates

Cada template inclui:

1. **Informações estruturadas:** Campos específicos que o agente precisa
2. **Critérios de aceitação:** Como saber quando está completo
3. **Contexto técnico:** Orientações para implementação correta
4. **Exemplos de código:** Padrões a seguir na implementação

Isso permite que o agente Copilot:
- Entenda exatamente o que fazer
- Implemente seguindo a arquitetura do projeto
- Faça validações apropriadas
- Adicione testes quando necessário

---

## 📚 Recursos Adicionais

- [Documentação do Sistema](../../docs/README.md)
- [Arquitetura do Projeto](../../docs/README.md#-arquitetura)
- [Como Executar Localmente](../../docs/README.md#-configuração-e-execução)

---

## 🆘 Precisa de Ajuda?

Se você não tem certeza de qual template usar ou tem dúvidas:

1. Verifique a [Documentação](../../docs/README.md)
2. Procure issues similares já criadas
3. Crie uma issue em branco com todos os detalhes que você tem
4. Entre em contato com a equipe de desenvolvimento

---

**Última atualização:** Outubro 2024
