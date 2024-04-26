# Exemplo de Design de Arquitetura

![MVC](https://github.com/ElgenneniF/MVC-ponderada/blob/f1332c8471f6ca4c55ff0c6b55731f84dabaf6c7/MVC.png)

- Nome do Projeto: Code Conecting Cultures
- Descrição: 
- Arquitetura: MVC (Model-View-Controller)
- Ferramenta de Diagramação: Kitt, Canva

### Modelos (Models):
-Os Models representam a estrutura de dados do aplicativo e a lógica de negócios relacionada a esses dados. Eles se comunicam com o Servidor Banco de Dados. Os modelos incluem:

  - User: Com campos como id, type, name, email, password, group_id, birthday, country_pov, country_of_birth e gender.
  - Group: Com campos como id, name, users_id e tutor_id.
  - Feedback: Com campos como id, content, from_user_id, to_user_id e group_id.
### Controladores (Controllers):
Os Controllers gerenciam a lógica do aplicativo e processam a entrada do usuário, encaminhando para o modelo ou visão adequados. Eles incluem:

  - User Controller: Gerencia as operações dos usuários com ações como Create, Read e Update.
  - Group Controller: Gerencia operações relacionadas a grupos com ações como Create, Read, Update e Delete.
  - Feedback Controller: Gerencia feedbacks com ações como Create, Read, Update e Delete.

### Views (Views):
As Views são a interface com o usuário, onde a saída do aplicativo é representada. Eles são renderizados pelo framework Sails.js e incluem:

  - Homepage: A página inicial do site.
  - navbar: A barra de navegação do site.
  - profiles: Perfis dos usuários.
  - group_members: Membros do grupo.
  - game_info: Informações sobre jogos.
  - game_indicators: Indicadores dos jogos.
  - logo: O logotipo do aplicativo.
  - Feedback: Página de feedback com os seguintes elementos:
      - form_questions: O formulário de perguntas de feedback.
      - submit: Botão para enviar feedback.
      - my_feedbacks: Feedbacks enviados pelo usuário.
      - logo: O logotipo do aplicativo repetido.

### Infraestrutura:
  - Render: Indica que o banco de dados está renderizando os modelos.
  - DBeaver: Representa a ferramenta de gerenciamento de banco de dados.

A comunicação entre os elementos é indicada pelas setas que mostram como o usuário interage com as Views, que por sua vez são controladas pelos Controllers, e estes manipulam os Models que se comunicam com o banco de dados.
