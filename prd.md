Product Requirements Document (PRD): EvoluFeed

Versão: 1.0
Status: Rascunho
Produto: Plataforma de Acompanhamento para Endocrinologia

1. Visão Geral e Problema

Produto: EvoluFeed é uma plataforma SaaS (Software as a Service) B2B, vendida para médicos e clínicas de endocrinologia com foco em emagrecimento. A plataforma é composta por dois módulos:

Portal do Médico (Web): Um dashboard para o profissional monitorar, gerenciar e interagir com seus pacientes.

App do Paciente (Mobile-Web/PWA): Uma rede social privada e um diário de progresso que conecta o paciente ao seu médico e a outros pacientes da mesma clínica.

Problema a ser Resolvido:

Para o Paciente: O tratamento de emagrecimento é uma jornada solitária e difícil. Pacientes perdem a motivação entre as consultas, têm dificuldade em manter a adesão à dieta e não têm um canal ágil para feedback ou um senso de comunidade.

Para o Médico: Falta de visibilidade. O médico só descobre o que aconteceu com o paciente semanas ou meses depois, na consulta de retorno. Isso dificulta ajustes rápidos no tratamento, reduz a adesão e limita as taxas de sucesso.

Solução (A Proposta de Valor):
O EvoluFeed cria um loop de feedback contínuo. Ele transforma o tratamento em uma jornada gamificada e social (para o paciente) e fornece ao médico uma ferramenta de monitoramento em tempo real (baseada nos dados de doc-page.html e index.html).

2. Personas

Persona 1: O Cliente (Médico)

Nome: Dra. Ana Beatriz

Profissão: Endocrinologista, dona de sua própria clínica.

Idade: 42

Objetivo: Aumentar a taxa de sucesso e retenção dos seus pacientes de emagrecimento.

Frustração: "Meus pacientes chegam motivados, mas eu sinto que os 'perco' no dia a dia. Quando eles voltam 2 meses depois e não seguiram o plano, é frustrante para nós dois. Eu preciso de uma forma de mantê-los engajados e ver o que estão comendo."

Persona 2: O Usuário Final (Paciente)

Nome: Ricardo Mendes

Profissão: Analista de TI

Idade: 35

Objetivo: Perder 25kg. Já tentou várias dietas, mas sempre desiste.

Frustração: "Eu me sinto sozinho nessa. É difícil manter o foco quando ninguém ao meu redor está na mesma situação. Eu gostaria de ter um 'check-in' mais rápido com a Dra. Ana e ver que não sou o único lutando."

3. Requisitos Funcionais (Core Features)

As features são baseadas nos mockups fornecidos.

Módulo 1: App do Paciente (Baseado em index.html)

O paciente só tem acesso ao se cadastrado pelo médico. Ele só vê posts e interage com pacientes do mesmo médico.

Feature: Feed Social (#inicio)

Descrição: Tela principal no estilo Instagram. Mostra um feed cronológico de posts (refeições) de todos os pacientes daquela clínica.

User Stories:

Como paciente, quero ver os posts de refeição de outros pacientes para me sentir parte de uma comunidade e ter ideias de pratos.

Como paciente, quero poder "Curtir" (ícone de coração) um post.

Como paciente, quero poder ver os comentários e adicionar um comentário em um post.

Como paciente, quero ver claramente os comentários do meu médico (ex: com um selo [Médico]).

Feature: Adicionar Post (#add-post)

Descrição: O "botão +" central para registrar uma refeição.

User Stories:

Como paciente, quero tirar uma foto ou fazer upload de uma foto da minha refeição.

Como paciente, quero selecionar o tipo de refeição (Café da Manhã, Almoço, etc.).

Como paciente, quero escrever uma legenda sobre a refeição ou como me senti.

(Sugestão) Como paciente, quero poder marcar um post como "Exceção" (para sinalizar ao médico que foi uma saída da dieta).

Feature: Acompanhamento de Peso (#peso)

Descrição: Uma tela para registrar o peso e ver o histórico.

User Stories:

Como paciente, quero inserir meu peso atual (em kg).

Como paciente, quero ver uma lista do meu histórico de pesagens com as datas.

Feature: Metas (#metas)

Descrição: Visualização das metas definidas pelo médico.

User Stories:

Como paciente, quero ver minhas metas principais (ex: Peso Alvo, Água Diária, Atividade Física) para me manter focado.

Feature: Perfil (#perfil)

Descrição: Minha página de perfil e informações.

User Stories:

Como paciente, quero ver minhas estatísticas (ex: Refeições postadas, Peso Inicial, Peso Meta).

Como paciente, quero ver a data e hora da minha próxima consulta.

Como paciente, quero poder ver meus exames solicitados.

Feature: Chat (Ícone de Mensagem)

Descrição: Um chat 1-a-1 direto com a clínica/médico.

User Stories:

Como paciente, quero enviar uma mensagem rápida para meu médico ou secretária para tirar dúvidas.

Módulo 2: Portal do Médico (Baseado em doc-page.html)

Feature: Dashboard (#dashboard)

Descrição: A "home" do médico, com uma visão geral da clínica.

User Stories:

Como médico, quero ver KPIs (Cards) do dia (ex: Consultas Hoje, Pacientes Ativos, Alertas).

Como médico, quero ver minha lista de "Próximas Consultas" com um status rápido do paciente (ex: "Ana Clara (-1.2kg)").

Como médico, quero ver um feed de "Atividade Recente" (ex: novos pesos, novas refeições, alertas de ganho de peso).

Feature: Feed de Pacientes (#feed)

Descrição: O "Instagram" do médico. Um feed unificado de todos os posts de todos os seus pacientes.

User Stories:

Como médico, quero rolar um feed único para monitorar a adesão dos meus pacientes.

Como médico, quero poder comentar em um post de paciente para dar feedback (ex: "Ótima escolha!" ou "Lembre-se da proteína.").

Como médico, quero poder "Curtir" um post como forma de incentivo.

Como médico, quero poder filtrar o feed (ex: ver posts marcados como "Exceção").

Feature: Agenda (#agenda)

Descrição: Calendário de consultas.

User Stories:

Como médico, quero ver minha agenda em formato de calendário mensal.

Como médico, quero ver os compromissos do dia em formato de lista.

Feature: Lista de Pacientes (#pacientes)

Descrição: O "CRM" de pacientes.

User Stories:

Como médico, quero ver uma lista de todos os meus pacientes ativos.

Como médico, quero poder buscar um paciente pelo nome.

Como médico, quero ver colunas rápidas de status (Progresso 30d, Adesão, Próx. Consulta).

Como médico, quero clicar em "Ver Prontuário" para abrir o perfil detalhado.

Feature: Prontuário do Paciente (#prontuário)

Descrição: A visão 360º de um paciente específico.

User Stories:

Aba (Dados do App): Como médico, quero ver apenas os posts do diário alimentar (fotos) e o histórico de peso daquele paciente.

Aba (Resumo Clínico): Como médico, quero escrever e ler minhas anotações clínicas privadas (anamnese, exames físicos, conduta).

Aba (Plano Alimentar): Como médico, quero fazer upload do PDF do plano alimentar para o paciente acessar no app dele.

Aba (Exames): Como médico, quero fazer upload e ver os resultados de exames do paciente.

4. Tiers do Produto (Seu Requisito Chave)

Aqui está a definição dos 3 modelos de produto que você mencionou:

Tier 1: "Community" (O Modelo Estático)

Foco: Engajamento e monitoramento social.

Descrição: O médico compra o acesso "como está" (as-is). Ele não pode mudar nada. É focado 100% na "rede social" de acompanhamento.

Features Inclusas:

App do Paciente: Completo (Feed, Postar, Peso, Perfil).

Portal do Médico:

Feature: Feed de Pacientes (para monitorar e comentar).

Feature: Lista de Pacientes (para gerenciar quem tem acesso).

Features Excluídas (Não inclusas):

Sem Dashboard de métricas.

Sem Agenda.

Sem Prontuário Eletrônico (Resumo Clínico, Planos, Exames).

Sem Chat 1-a-1.

Sem customização de logo ou cores.

Tier 2: "Clinic" (O Modelo com Customização)

Foco: Gestão completa da jornada do paciente.

Descrição: O "carro-chefe". Inclui todas as features de gestão e permite customização básica da marca.

Features Inclusas:

Tudo do Tier 1, MAIS:

Portal do Médico:

Feature: Dashboard completo.

Feature: Agenda completa.

Feature: Prontuário do Paciente completo (todas as abas).

App do Paciente:

Feature: Chat 1-a-1 habilitado.

Customizações Inclusas:

Médico pode subir o logo da clínica (que aparece no portal e no app).

Médico pode definir a cor primária do app (ex: o seu #A2574F).

Médico pode customizar as Metas (ex: adicionar "Horas de Sono").

Tier 3: "Enterprise" (O Modelo 100% Customizado / White-Label)

Foco: Solução completa para grandes clínicas, franquias ou parceiros.

Descrição: O produto é "re-empacotado" com a marca do cliente.

Features Inclusas:

Tudo do Tier 2, MAIS:

White-Label Completo: O app é publicado na App Store/Play Store com o nome e marca da Clínica. O portal web fica em um domínio customizado (ex: app.clinicaanabeatriz.com).

Gestão Multi-Médico: Um perfil "Admin" da clínica pode gerenciar múltiplos médicos, onde cada médico só vê seus próprios pacientes.

Analytics Avançados: Relatórios de performance da clínica (adesão média, perda de peso total, etc.).

Acesso API: Para integração com sistemas de EMR ou agendamento existentes.

Suporte Prioritário e Onboarding dedicado.

5. Requisitos Não-Funcionais

Segurança (Crítico): A plataforma deve ser compatível com a LGPD (Lei Geral de Proteção de Dados).

Todos os dados de pacientes devem ser criptografados (em trânsito e em repouso).

Silo de Dados: Um paciente SÓ PODE ver posts de outros pacientes da mesma clínica. Pacientes da Clínica A NUNCA podem ver dados da Clínica B.

Performance: O carregamento das imagens no feed (paciente e médico) deve ser rápido. Usar otimização e lazy-loading.

Plataforma:

App Paciente: Deve ser um PWA (Progressive Web App) para começar (baseado no index.html), para evitar custos de loja de app.

Portal Médico: Web-App responsivo (baseado no doc-page.html).

Dados: Os mockups usarão dados "fake", mas a arquitetura final deve usar um banco de dados real (ex: Firestore, PostgreSQL).

6. Roadmap Futuro (Próximos Passos)

Gamificação: Introduzir pontos, streaks (dias seguidos de posts) e medalhas por atingir metas (ex: "Medalha de 5kg").

Comunidade 2.0: Criar "Tópicos" dentro da comunidade (ex: #receitas, #dificuldades) para os pacientes interagirem além dos posts de refeição.

Integrações: Conectar com balanças inteligentes (ex: Withings) e apps de atividade (Google Fit, Apple Health) para automatizar os registros.
