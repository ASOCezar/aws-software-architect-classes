# IAM (Identity and Access Management)

## Conceito

Permite a configuração do nível de acesso de usuários e serviços em uma infraestrutura AWS.

É possível fazer a configuração de acesso separado por Usuários, Grupos, Funções(roles) e Permissões.
 - Usuários: Criação de acesso a usuários individuais.
 - Grupos: Criação de acesso a grupos (conjunto de usuários).
 - Roles: Criação de acesso temporário de um serviço a outro serviço AWS.
 - Permissões: Referente a atribuição de acesso e direito a leitura e/ou escrita (policies) que é fornecida a Usuários, Grupos ou Roles.

Ao criar um usuário é possível atribuir permissões herdadas de grupos ou outro usuário ou ainda atribuir manualmente as devidas permissões. Todo usuário criado possui uma URL própria de acesso que permite o login de maneira direta no navegador. 
Há duas formas possíveis de acesso (pode ser definido a possibilidade do acesso): 
  - Acesso de um usuário à AWS através do console: para isso é necessário que o usuário saiba apenas seu nome de usuário e senha.
  - Acesso programático, que exige chave de acesso e chave secreta da API.

Todas as informações de usuário são acessíveis apenas no momento da criação deste. Por isso é importante que se armazene essas informações em local seguro.

Ao criar uma nova conta na AWS é automaticamente gerado o usuário root daquele console. No entanto, é **altamente** recomendável que se crie novos usuários e lhes atribua as devidas permissões para fazer qualquer forma de utilização de serviços dentro da AWS. 

Sendo assim, é possível que se crie um grupo administrador, com todas as permissões, através do IAM atribuindo manualmente a policy AdministratorAccess. Dessa forma, será possível inserir novos usuários nesse grupo de administradores.