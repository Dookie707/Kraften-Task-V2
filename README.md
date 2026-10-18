# Kraften Task

Protótipo navegável de um sistema SaaS de gestão de projetos, tarefas e setores, com quatro perfis: Super Admin, CEO, Gestor e Funcionário.

**Demonstração:** https://kraften-task.vercel.app

## O que o protótipo mostra
- Projetos e tarefas com responsáveis em ordem, descrição e prazo de cada um
- Etapas entre setores em sequência ou em paralelo, com aceite do Gestor participante
- Status de execução, bloqueio com justificativa e farol de prazo calculado
- Visão geral por perfil com indicadores clicáveis
- Calendário (mês, semana e dia) com filtros
- Análises e desempenho para CEO (todos os setores) e Gestor (próprio setor)
- Aprovação de projetos criados por funcionários
- Exportação em PDF das listagens, do calendário e do relatório de análises

## Como rodar
É um único arquivo HTML, sem build.

1. Abra `index.html` no navegador, ou
2. Sirva a pasta com qualquer servidor estático, por exemplo:

```bash
npx http-server -p 8080
```

Na tela inicial, escolha um usuário para entrar. Os dados são fictícios e ficam salvos no navegador (localStorage). O botão "Restaurar dados de demonstração" volta ao estado inicial.

## Limitações do protótipo
- Não há servidor, banco de dados nem login real; cada navegador tem sua própria cópia dos dados.
- Parte das análises (tendências, tempos por setor, categorias de bloqueio) usa histórico simulado.

## Tecnologia
HTML, CSS e JavaScript puro. Bibliotecas carregadas por CDN: jsPDF e jsPDF-AutoTable (exportação em PDF). Fonte Poppins (Google Fonts).