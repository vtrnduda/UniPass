### **RF034 \- Visualizar Logs do Sistema**

Como administrador, gostaria de visualizar logs de ações realizadas pelos usuários comuns, para garantir rastreabilidade e transparência.

Amanda, administradora, precisa investigar uma reclamação sobre reservas canceladas indevidamente.  
Ela acessa o sistema UniPass pelo computador da administração.  
Amanda faz login com sua matrícula e senha.  
Na barra lateral, ela clica em "Administração" no menu.  
No painel administrativo, ela clica em "Auditoria e Logs".  
O sistema exibe uma tela de busca com filtros:  
  \- Período: últimas 24h, 7 dias, 30 dias, personalizado  
  \- Usuário: campo para CPF ou nome  
  \- Ação: dropdown com tipos (Login, Reserva, Cancelamento, etc.)  
  \- Módulo: Cadastro, Transporte, Comunicação, etc.  
Amanda filtra por:  
  \- Período: "Últimos 7 dias"  
  \- Ação: "Cancelamento de reserva"  
  \- Deixa usuário em branco para ver todos  
O sistema exibe uma tabela com resultados:

  Data/Hora | Usuário | Ação | Detalhes | IP | Status  
  27/07 08:15 | Maria Silva (\*\*\*456\*\*\*) | Cancelou reserva | Rota Centro-UEPB, 28/07 07:30 | 192.168.1.10 | Sucesso  
  26/07 15:30 | João Santos (\*\*\*789\*\*\*) | Cancelou reserva | Rota IFPB-Centro, 27/07 14:00 | 10.0.0.25 | Sucesso  
  26/07 07:15 | Ana Costa (\*\*\*123\*\*\*) | Tentou cancelar | Rota Centro-UFPB, 26/07 07:30 | 172.16.0.5 | Falhou: Fora do prazo

Amanda clica em uma linha específica para ver detalhes completos.  
O sistema exibe informações detalhadas:  
  \- Timestamp completo: "27/07/2025 08:15:23.456"  
  \- CPF do usuário: "123.456.789-00" (completo para admin)  
  \- Sessão: ID único da sessão do usuário  
  \- User-Agent: informações do dispositivo/navegador  
  \- Justificativa do cancelamento: "Compromisso médico urgente"  
  \- Ação do sistema: "Vaga liberada automaticamente"  
  \- Impacto: "Lista de espera notificada"  
Amanda pode exportar os logs clicando em "Exportar CSV".  
O sistema gera um arquivo com todos os registros do período filtrado.  
Para preservar privacidade, logs mais antigos que 1 ano são automaticamente anonimizados.