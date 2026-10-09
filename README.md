# Zuno — Gestão de Atividades, Horas e Clientes

Sistema completo para gestão de agendas, controle e apontamento de horas (*timesheets*), acompanhamento de projetos e relacionamento com clientes, com integração em tempo real na nuvem através do **Supabase**.

---

## 🚀 Funcionalidades

- **Agenda & Calendário:** Visualização semanal, mensal e quadro da equipe por colaborador, com filtros de clientes, status e urgência.
- **Apontamento de Horas:** Controle detalhado de horas trabalhadas por projeto e cliente com totalizadores diários/semanais.
- **Empresas & Clientes:** Cadastro completo com histórico, fotos, contatos e horas contratadas vs. executadas.
- **Gestão de Projetos:** Controle orçamentário em minutos, prazos e entregas.
- **Dashboard & Relatórios:** Indicadores gráficos de desempenho e exportação personalizada em CSV e PDF.
- **Comunicação com Cliente:** Checklist de rotinas e acompanhamento operacional semanal.
- **Gerador de Confirmação:** Criação de artes visuais em Canvas (1080x1080) para confirmação de reuniões via WhatsApp.
- **Thalia (Assistente Executiva Integrada):**
  - Comandos por voz e texto com síntese de voz (TTS) e reconhecimento de fala (STT).
  - Processamento de linguagem natural (NLP local) para agendamentos, briefings diários e alertas de reuniões.

---

## ☁️ Integração com Supabase (Nuvem)

O Zuno possui sincronização automática em tempo real com o **Supabase**:
- **Cache Local + Nuvem:** O sistema inicializa instantaneamente pelo cache local e sincroniza com o banco de dados em segundo plano.
- **Realtime:** Atualizações em tempo real via WebSockets (qualquer alteração feita por um membro da equipe é refletida automaticamente nos outros dispositivos).
- **Tabelas Utilizadas:**
  - `zuno_companies`: Cadastro de empresas/clientes.
  - `zuno_activities`: Compromissos e tarefas da agenda.
  - `zuno_hours`: Apontamentos de horas.
  - `zuno_projects`: Projetos e orçamentos.
  - `zuno_users`: Usuários e colaboradores.
  - `zuno_comm`: Checklists de comunicação.
  - `zuno_settings`: Metas e configurações globais.
  - `zuno_notes`: Bloco de anotações compartilhadas.
  - `zuno_todos`: Tarefas pendentes.

---

## 💻 Como Executar

Por ser uma Single Page Application autocontida:
1. Abra o arquivo `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox, Brave).
2. Não requer instalação de servidor web local ou compilação de código.
3. Para acesso online da equipe, o repositório pode ser publicado diretamente no **GitHub Pages**, **Vercel** ou **Netlify**.

---

## 📁 Estrutura de Arquivos

- `index.html`: Arquivo principal da aplicação pronto para deploy e execução web.
- `Zuno_Computador (4).html`: Cópia executável local com o mesmo código.
- `README.md`: Documentação do sistema e do banco de dados.
- `.gitignore`: Arquivos ignorados pelo controle de versão.
