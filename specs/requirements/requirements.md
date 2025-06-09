# Requisitos de Software
---

UniPass: Sistema de Gerenciamento de Transporte Universitário  
Versão 1.2  
---

## Histórico de revisões

---

| Data | Versão | Descrição | Autor |
| ----- | ----- | ----- | ----- |
| 24/05/2025 | 1.0 | Entrega inicial do documento de visão | Equipe UniPass |
| 07/06/2025 | 1.1 | Desenvolvimento inicial do documento com os requisitos de software | Equipe UniPass |
| 08/06/2025 | 1.2 | Atualização dos requisitos funcionais | Equipe UniPass |

## Sumário

- [Requisitos de Software](#requisitos-de-software)
  - [Histórico de revisões](#histórico-de-revisões)
  - [Sumário](#sumário)
- [Introdução](#introdução)
  - [Definições, Acrônimos e Abreviações](#definições-acrônimos-e-abreviações)
- [Usuários identificados](#usuários-identificados)
- [Requisitos funcionais](#requisitos-funcionais)
- [Requisitos não-funcionais](#requisitos-não-funcionais)
  - [Disponibilidade](#disponibilidade)
  - [Privacidade e segurança](#privacidade-e-segurança)
  - [Usabilidade](#usabilidade)
  - [Suportabilidade](#suportabilidade)
  - [Interoperabilidade](#interoperabilidade)
  - [Manutenibilidade](#manutenibilidade)
  - [Desempenho](#desempenho)
  - [Implementação](#implementação)
  - [Implantação](#implantação)
- [Não requisitos](#não-requisitos)
---

# Introdução

---

## O objetivo deste documento é apresentar os requisitos de software do produto UniPass, voltado para a gestão eficiente e segura do transporte gratuito de estudantes universitários.

Definições, Acrônimos e Abreviações  
---

Esta subseção fornece as definições de todos os termos, acrônimos e abreviações necessárias à adequada interpretação do Documento de Requisitos.

**Identificação dos requisitos**: por convenção, a referência a requisitos é feita através do identificador de requisitos, conforme descrito abaixo:

* **RF** \- Requisito Funcional  
* **RNF** \- Requisito Não-Funcional  
* **NR** \- Não Requisito

O identificador do requisito será uma sequência numérica única.  
Exemplo: RF001, RNF002, NR001

**Atributos dos Requisitos**: 

* **Requisitos vinculados**: rastreabilidade com outros requisitos.  
* **Prioridade**: Essencial, Importante, Desejável.  
* **Complexidade**: Complexa, Alta, Média ou Baixa.  
* **Risco**: Alto, Médio, Baixo. 

Usuários identificados  
---

Os seguintes usuários foram identificados para o sistema UniPass:

* Usuário do sistema  
  * Usuários comuns  
    * Estudantes universitários  
    * Motoristas do transporte intermunicipais  
    * Atendente de Suporte  
    * Agente administrativo   
  * Administrador do sistema

Requisitos funcionais  
---

Os requisitos funcionais são descritos a seguir.

* **\[RF001\]** \- Como estudante, gostaria de  solicitar o meu cadastro no sistema UniPass.  Devo fornecer de maneira obrigatória o meu nome completo, RG, CPF, data de nascimento, universidade/ Campus em qual estudo, turno das aulas, declaração de vínculo com a instituição de ensino, comprovante de residência e previsão de conclusão de curso. 

* **\[RF002\]** \- Como estudante, quero anexar documentos em formatos PDF, .jpg ou .png, durante o processo de cadastro ou atualização do meu perfil. Para comprovar minha matrícula, residência ou outras informações exigidas.

* **\[RF003\]** \- Como agente administrativo, gostaria de poder validar ou reprovar cadastros de estudantes, verificando a autenticidade dos documentos enviados, com base nos critérios estabelecidos (vínculo ativo com uma universidade, residência no município, relação dos dados pessoais fornecidos com o titular solicitante)

* **\[RF004\]** \- Como estudante, gostaria de poder cancelar meu benefício.

* **\[RF005\]** \- Como estudante, gostaria de poder solicitar a emissão da carteirinha física em casos casos de perda.

* **\[RF006\]** \- Como estudante, quero poder receber mensagens importantes emitidas pela secretaria de transporte por e-mail e pelo aplicativo. Ex: Status da solicitação de cadastro.

* **\[RF007\]** \- Usuário Comum, quero poder reportar problemas com o sistema ao suporte.

* **\[RF008\]** \- Como agente administrativo, quero poder enviar mensagens importantes emitidas pela secretaria de transporte para e-mail e para os aplicativos dos demais usuários do sistema. Ex: Status da solicitação de cadastro.

* **\[RF009\]** \- Como estudante, desejo ser capaz de editar meus dados pessoais e atualizar meus documentos sempre que necessário.

* **\[RF010\]** \- Como usuário comum, eu gostaria de ter acesso pela interface do sistema a rota a qual o ônibus irá seguir, a localização em tempo real,  uma lista de universidades onde o ônibus deve passar e a quantidade de estudantes confirmados por universidade no ônibus.

* **\[RF011\]** \- Como estudante, gostaria de registrar a intenção de utilizar o transporte universitário, selecionando o ônibus relacionado ao turno e instituição a qual informei em meu cadastro **\[RF001\]** sem a necessidade de justificar a ação, e escolhendo entre as opções “ida e volta”, “apenas ida” ou “apenas volta”.

* **\[RF012\]** \- Como estudante, gostaria de registrar a intenção de utilizar o transporte universitário, selecionando o ônibus relacionado ao turno e instituição adversa a qual informei em meu cadastro **\[RF001\]** justificando a necessidade da ação (texto a ser registrado no sistema), e escolhendo entre as opções “ida e volta”, “apenas ida” ou “apenas volta”.

* **\[RF013\]** \- Como estudante, gostaria de cancelar a intenção de utilizar o transporte universitário, selecionando o ônibus relacionado ao turno e instituição a qual realizei a demonstração de interesse previamente **\[RF001\]** com a necessidade de justificar a ação  (texto a ser registrado no sistema).

* **\[RF014\] \-** Como administrador do sistema, gostaria de definir o tempo mínimo e máximo que a intenção ou cancelamento de uso de um aluno deve ser feita. Bloqueando qualquer tentativa de reserva antes ou depois deste tempo.

* **\[RF015\]** \-  Como estudante, gostaria de escolher em qual assento disponível ficarei no ônibus, ao reservar minha vaga.

* **\[RF016\]** \- Como estudante, gostaria de abrir solicitação para reservar vaga em turno diferente, mediante comprovação.

* **\[RF017\]** \- Como administrador do sistema, gostaria de poder extrair relatórios Xls / Csv para obter informações sobre a utilização do transporte, como: tempo de percurso, número de reservas por dia, frequência dos estudantes. 

* **\[RF018\]** \- Como agente administrativo, gostaria de ter conhecimento da frequência de cada estudante cadastrado no sistema, bem como faltas não justificadas.

* **\[RF019\]** \- Como estudante, motorista e agente administrativo, gostaria de  reportar problemas técnicos, sugestão de melhoria ou denúncias, com acompanhamento do status da solicitação e resposta da equipe responsável (suporte ou administrador)

* **\[RF020\]** \- Como agente administrativo, gostaria de visualizar em tempo real a quantidade de alunos que fizeram/cancelaram a reserva.

* **\[RF021\]** \- Como agente administrativo, gostaria de revogar benefício, alterar dados ou cadastrar alunos dentro do sistema exigindo o mesmo escopo de dados presentes no **RF001**, mediante justificativa (texto a ser registrado no sistema).

* **\[RF022\]** \- Usuário do sistema, gostaria de saber o horário definido para a partida, em um determinado turno, a partir de um ponto de embarque definido dentro do município sede da secretaria.

* **\[RF023\]** \- Usuário do sistema, gostaria de saber o horário definido para a partida, em um determinado turno, a partir de um ponto de embarque definido próxima a uma determinada instituição dentro da rota relacionada ao ônibus.

* **RF024\]** \- Como agente administrativo, gostaria de gerenciar as rotas e horários do transporte, definindo itinerários, pontos de parada.

* **RF025\]** \- Como agente administrativo, gostaria de ser notificado caso um ônibus tenha a sua capacidade máxima atingida.

* **\[RF026\]** \- Como motorista, gostaria de registrar ocorrências e manter contato direto com o administrativo em casos de necessidade através de uma ala de mensagens.                                        

* **\[RF027\]** \- Como estudante, gostaria de acompanhar o status de confirmação de reservas, alterações de rota, tempo limite de reserva para uma vaga e quantidade de vagas remanescentes.

* **\[RF028\]** \- Como atendente de suporte, gostaria de visualizar o nome do solicitante e qual o tipo de ocorrência solicitada.

* **\[RF029\]** \- Como estudante, gostaria de consultar o histórico das minhas viagens realizadas, incluindo datas, horários e rotas utilizadas, para acompanhar meu uso do benefício.

* **\[RF030\]** \- Como administrador do sistema, quero gerenciar permissões de acesso para cada tipo de usuário.

* **\[RF031\]** \- Como usuário comum, gostaria de verificar quais as regras de privacidade e uso de dados de maneira resumida e simplificada, para que eu possa ter uma experiência mais segura. As regras de privacidade e uso de dados também devem ser apresentadas em uma página de termos de uso e política de privacidade, que deve ser acessível a partir do rodapé do site, a partir da página de cadastro e da página de regras simplificadas.

* **\[RF032\] \-** Como estudante, gostaria de acessar minha carteirinha digital no aplicativo UniPass para validar meu embarque no transporte mesmo sem conexão com a internet. A carteirinha deve conter minha foto, nome, número de matrícula, turno autorizado, universidade e código NFC para leitura na catraca.

* **\[RF033\] \-** Como estudante, gostaria de visualizar a lotação atual do ônibus da minha rota, para saber se ainda há vagas disponíveis. A informação deve ser atualizada automaticamente a cada nova reserva ou cancelamento.

* **\[RF034\]** \- Como administrador, gostaria de visualizar logs de ações realizadas pelos usuários comuns, para garantir rastreabilidade e transparência.

* **\[RF035\]** \- Como estudante que perdeu o prazo de renovação da carteirinha, gostaria de abrir solicitação para reativação emergencial do meu cadastro apresentando justificativa válida.

* **\[RF036\]** \- Como estudante, quando não houver vagas disponíveis para o ônibus com a rota para minha universidade, gostaria de entrar em lista de espera e automaticamente ser alocado para uma vaga em caso de desistência e outros estudantes.

* **\[RF037\]** \- Como estudante, gostaria de visualizar as regras de uso do transporte e o regulamento de forma clara e acessível dentro do aplicativo.

* **\[RF038\]** \- Como administrador, gostaria de ativar ou desativar funcionalidades específicas do sistema, conforme necessidades operacionais ou mudanças de políticas.

* **\[RF039\]** \- Como administrador, gostaria que o sistema realizasse a verificação sobre se atende aos requisitos mínimos de hardware e software para a execução do sistema, e caso não atenda, deve exibir uma mensagem de erro informando o motivo.

* **\[RF040\]** \- Como administrador, gostaria de configurar períodos de renovação baseados no calendário acadêmico das universidades, definindo prazos automáticos para solicitação de documentos atualizados.

* **\[RF041\]** \- Como estudante, gostaria de ser capaz de me logar no sistema. As informações necessárias para o login são CPF e senha.

* **\[RF042\]** \- Como administrador, motorista e agente administrativo , gostaria de ser capaz de me logar no sistema. As informações necessárias para o login são a matrícula do servidor e senha.

* **\[RF043\]** \- Como administrador, gostaria de poder criar um novo perfil para agentes administrativos. As informações necessárias são nome completo, matrícula do funcionário. Também deve ser definido neste momento uma chave de acesso.

* **\[RF044\]** \- Como estudante, gostaria de criar um perfil no sistema. As informações necessárias para a criação serão  CPF e uma senha a ser definida.

* **\[RF045\]** \- Como agente administrativo eu gostaria de separar por turno qual usuário irá receber as mensagens por mim enviadas. Se de todos os turnos, apenas os estudantes da manhã, ou apenas da tarde ou apenas da noite.

* **\[RF046\]** \- Como agente administrativo eu gostaria de programar mensagens para serem enviadas em determinada data e hora do dia a serem definidas por mim.

Requisitos não-funcionais  
---

Os requisitos não-funcionais são descritos a seguir.

Disponibilidade  
---

* **\[RNF100\]** \- O sistema deve estar disponível 24 horas por dia, 7 dias por semana,com janelas de manutenção programadas apenas em horários de menor uso (madrugada)

* **\[RNF102\]** \- O sistema deve suportar operação com 10 mil acessos simultâneos sem perda de disponibilidade.

* **\[RNF103\]** \- O sistema deve ser projetado com foco em escalabilidade, permitindo expansão de recursos como armazenamento e processamento, sem comprometer a disponibilidade ou desempenho das funcionalidades oferecidas.

Privacidade e segurança  
---

* **\[RNF200\]**\- O sistema deve contar com firewalls que impeçam ações potencialmente maliciosas dentro do aplicação.

* **\[RNF201\]** \- O sistema deve garantir que apenas usuários previamente cadastrados acessem ao sistema com suas devidas permissões.

* **\[RNF202\]** \- O sistema deve atender aos requisitos de privacidade da LGPD (Lei Geral de Proteção de Dados).

* **\[RNF203\]** \- O sistema deve ser desenvolvido de forma que os dados pessoais dos clientes sejam criptografados, como endereço de e-mail, senha, nome completo, cpf. A criptografia deverá ser realizada com o algoritmo SHA-512, e deve impossibilitar a recuperação dos dados originais.

* **\[RNF204\] \-**  O sistema deve definir políticas de inatividade automática, para que sessões sejam encerradas após um tempo sem uso requerendo um novo login.

* **\[RNF205\] \-**  O sistema deve realizar o backup dos dados dos clientes, para que eu possa recuperar os dados em caso de falha no sistema.

* **\[RNF206\]** \- Os termos de uso e política de privacidade do sistema devem se manter  atualizados conforme a legislação.

Usabilidade  
---

* **\[RNF300\]** \- 	O sistema deve conter feedback visual após cada ação, por exemplo em situações de carregamento, erro, sucesso.

* **\[RNF301\]** \- O sistema deve oferecer textos em linguagem acessível, evitando termos técnicos.

* **\[RNF302\]** \- O sistema deve seguir padrões de design responsivo, adaptando-se a telas de todos os tamanhos.

* **\[RNF303\]** \- O sistema deve ser acessível a pessoas com deficiência visual, auditiva e motora, adotando práticas de acessibilidade digital que garantam uma navegação inclusiva e eficiente.

* **\[RNF304\]** \- O sistema deve oferecer uma experiência de uso simples e intuitiva, permitindo que qualquer usuário consiga navegar e utilizar suas funcionalidades de forma autônoma, sem a necessidade de capacitação prévia.

Suportabilidade  
---

* **\[RNF400\]** \- O sistema deve ser desenvolvido de forma que possa ser executado nos três principais navegadores da web: Google Chrome, Mozilla Firefox e Microsoft Edge através de um computador com sistema operacional Windows, Linux ou Mac OS, bem como tablets e smartphones com sistema operacional Android ou iOS.

* **\[RNF401\]** \- O sistema deve ser otimizado para ter um baixo consumo de memória Ram e rom do aparelho, exigindo o mínimo de 1gb Ram e 8gb de Rom

* **\[RNF402\]** \- O sistema deve ser compatível com versões 6.0 do android em diante, e versão 11.0.0 do IOS em diante

Interoperabilidade  
---

* **\[RNF500\]** \- O sistema deve gerenciar adequadamente situações de alta concorrência, como liberação de vagas, garantindo que o número correto de reservas seja aceito e evitando o “overselling”.

* **\[RNF501\]** \- O sistema deve ser integrado com a API RESTful, permitindo integrações com sistemas, como Google Maps, para mapeamento das rotas itinerárias.

*  **\[RNF502\] \-** Garantir que a logística de status do sistema se reflita no sistema de catracas.

Manutenibilidade  
---

* **\[RNF600\]** \- O sistema deve ser desenvolvido seguindo os padrões estabelecidos pelo clean code.

* **\[RNF601\]** \- O sistema deve ser desenvolvido de forma que possa ser facilmente testado e validado, com testes previamente escritos e automatizados.

* **\[RNF602\]** \- O sistema deve ser construído de modo que possibilite integração com outros sistemas da prefeitura.

Desempenho  
---

* **\[RNF700\]** \- O sistema deve ter um baixo consumo de dados móveis, utilizando de técnicas como o manter alguns dados em cache.

* **\[RNF701\]** \- O sistema deve responder a requisição dos usuários em no máximo 3 segundos para operações simples (login, consultas) e 10 segundos para operações complexas (geração de relatórios).

Implementação
---

* **\[RNF800\]** \- O sistema deve ser construído com arquitetura baseada em microsserviços.

* **\[RNF801\]** \- O sistema deve usar controle de versionamento de código via Git.

* **\[RNF802\]** \- O sistema deve seguir práticas de CI/CD para facilitar deploy contínuo.

Implantação  
---

* **\[RNF900\]** \- O sistema deve ser verificado quanto ao desempenho mínimo tolerado dos lados servidor e clientes. As especificações sobre pré-requisitos de hardware e software para a execução do sistema devem ser apresentadas em uma página de pré-requisitos, que deve ser acessível a partir do rodapé do site.

* **\[RNF901\]** \- O sistema deve ser verificado quanto ao desempenho mínimo tolerado dos lados servidor e clientes. As especificações sobre pré-requisitos de hardware e software para a execução do sistema devem ser apresentadas em uma página de pré-requisitos, que deve ser acessível a partir do rodapé do site.

* **\[RNF902\]** \- O sistema deve implementar sockets de comunicação para sincronizar com o sistema na catraca.

Não Requisitos  
---

* ***\[NR951\] \-*** Como motorista, gostaria de permitir a entrada de estudantes no ônibus em caso de sobra de vagas mediante a liberação dos mecanismos de catraca.