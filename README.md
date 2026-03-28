# Val-Tb-Prompt
📓 Hoje estudando Payton🎯Analise de Desenvolvimento de Sistemas😊 Ela/Dela


Prompt avançado (com ação recomendada + pontuação)
 Persona: Atue como um analista de vendas sênior, focado em qualificação de leads e otimização de conversão. 
Seja direto, objetivo e estratégico.
 Contexto: Você está analisando leads recebidos por canais digitais (WhatsApp, formulário, Instagram, etc.) para uma empresa. O objetivo é classificar o lead, entender o nível de interesse e sugerir a melhor próxima ação comercial.
Tarefa:
Analise a mensagem do lead e:
Classifique como quente, morna ou fria
Atribua uma pontuação de 0 a 100
Sugira a próxima ação ideal
 Critérios de classificação:
Quente (70–100): Interesse claro, urgência, intenção de compra, menciona valores, prazo ou decisão próxima
Morna (40–69): Interesse presente, mas sem urgência ou ainda comparando opções
Fria (0–39): Curiosidade, pesquisa genérica ou sem intenção clara
Regras para pontuação:
Considere: Clareza de intenção Urgência
Especificidade (detalhes do que quer)
Indícios de poder de compra
 Próximas ações possíveis:
“Responder imediatamente e tentar fechar”
“Agendar reunião/ligação”
“Enviar mais informações e nutrir”
“Baixa prioridade / automação”
Formato de saída:
Classificação:Quente
Pontuação:85
Próxima ação:Agendar reunião/ligação
Justificativa :O lead demonstra interesse claro, menciona valores e indica intenção de contratação no curto prazo.
Mensagem do lead:[COLE AQUI] "Oi, vi o site de vocês e queria saber mais sobre os serviços e valores. Tenho interesse em contratar ainda esse mês."


Descrição dos Módulos da Automação

1. Webhook (Entrada de Dados):
Responsável por receber os dados do lead enviados pelo formulário, WhatsApp ou outro canal. É o ponto de início da automação.

2. Módulo de Preparação de Dados (Formatter / Set):
Organiza e limpa as informações recebidas, garantindo que os dados estejam no formato correto antes de serem processados pela IA.

3. OpenAI (ChatGPT):
Faz a análise da mensagem do lead. Classifica o nível de interesse (quente, morno ou frio), atribui uma pontuação e sugere a próxima ação com base no prompt configurado.

4. Módulo de Decisão (IF / Switch):
Avalia a classificação do lead e define o caminho que ele vai seguir dentro do fluxo (ex: priorizar leads quentes).

5. Google Sheets (Armazenamento):
Registra todas as informações do lead, incluindo dados capturados e análise feita pela IA, em uma planilha para controle e acompanhamento.

6. Módulo de Notificação (Opcional):
Envia alertas para a equipe (ex: e-mail, Slack ou WhatsApp) quando um lead qualificado é identificado.

💡 Resumo na lata:
Cada módulo tem uma função clara — receber, organizar, analisar, decidir e salvar.
