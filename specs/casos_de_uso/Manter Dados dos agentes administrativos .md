**RF043**

História do Usuário \- Manter Dados dos agentes administrativos (Administrador)  
Carla como administrador acessa o sistema com sua matrícula e senha.

Ela navega até a seção "Cadastro de Agente" e seleciona "Novo Cadastro".

O sistema exibe um formulário com os campos obrigatórios:

Nome completo (com validação para evitar números/símbolos)

CPF (com máscara e validação automática)

Matrícula institucional

Data de nascimento (calendário interativo)

Turno (Manhã/Tarde/Noite)

Foto do agente (opcional, com pré-visualização)

 Carla preenche todos os campos e clica em "Salvar".

O sistema valida os dados e exibe a confirmação:  
✅ "Agente cadastrado com sucesso\! Nº de matrícula: 2025005678"

Fluxo Principal \- Edição de Cadastro  
 Carla pesquisa o agente pelo CPF ou nome na barra de busca.

O sistema mostra o registro completo com o botão "Editar". Ela atualiza o campo "Turno" (de Tarde para Noite) e clica em "Salvar".

O sistema exibe:  
🔄 "Registro atualizado. Histórico de alterações registrado."

Fluxo Alternativo 1 \- Campos Obrigatórios Não Preenchidos  
Se Carla esquecer de preencher o CPF, o sistema destaca o campo em vermelho com a mensagem:  
❌ \*"CPF é obrigatório. Formato: 000.000.000-00"\*  
 O botão "Salvar" permanece desativado até todos os campos obrigatórios serem preenchidos corretamente.

Fluxo Alternativo 2 \- CPF Já Cadastrado  
Ao tentar cadastrar um CPF já existente na base, o sistema exibe:  
⚠️ "CPF já registrado para o administrativo: João  (Matrícula: 2023001234). Deseja acessar o registro existente?"

Carla seleciona "Sim" e é redirecionada para o perfil do agente.

Fluxo Alternativo 3 \- Exclusão de Registro  
Carla localiza o agente e clica em "Excluir".

O sistema solicita confirmação:  
🗑️ \*"Tem certeza que deseja desativar o agente Luiza Oliveira (CPF: 123.456.789-00)?"\*

\# Após confirmar, o sistema remove o registro e exibe:  
✔️ "Registro excluído. Esta ação não pode ser desfeita."

