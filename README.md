# kayke-jordan4nb
Repositorio Back-End requisitado pelo nosso professor Afonso  


# Análise de Requisitos: Sistema de Autenticação de Usuários importante 

Este documento descreve a análise de requisitos para um sistema de autenticação de usuários. O objetivo é garantir que o sistema atenda às necessidades de segurança e usabilidade para autenticar usuários de forma eficaz.

## Índice

1. [Objetivo](#objetivo)
2. [Requisitos Funcionais](#requisitos-funcionais)
3. [Requisitos Não Funcionais](#requisitos-não-funcionais)
4. [Casos de Uso](#casos-de-uso)
5. [Requisitos de Segurança](#requisitos-de-segurança)
6. [Requisitos de Interface](#requisitos-de-interface)
7. [Considerações Finais](#considerações-finais)

## Objetivo

O objetivo deste sistema de autenticação é fornecer uma maneira segura e eficiente para os usuários acessarem suas contas. O sistema deve garantir que apenas usuários autorizados possam acessar recursos e dados restritos.

## Requisitos Funcionais

1. **Cadastro de Usuário**
   - O sistema deve permitir que novos usuários se registrem com um e-mail e uma senha.
   - O sistema deve enviar um e-mail de confirmação para o endereço fornecido durante o registro.

2. **Login de Usuário**
   - O sistema deve permitir que os usuários façam login com e-mail e senha.
   - O sistema deve validar a combinação de e-mail e senha com os dados armazenados.

3. **Recuperação de Senha**
   - O sistema deve permitir que os usuários solicitem a recuperação de senha por e-mail.
   - O sistema deve enviar um link de redefinição de senha para o e-mail fornecido.

4. **Logout de Usuário**
   - O sistema deve permitir que os usuários façam logout da sua conta.

5. **Gerenciamento de Sessões**
   - O sistema deve gerenciar e manter sessões de usuário ativas até que o logout seja realizado ou a sessão expire.

## Requisitos Não Funcionais

1. **Desempenho**
   - O sistema deve ser capaz de autenticar um usuário em menos de 2 segundos.

2. **Escalabilidade**
   - O sistema deve suportar um número crescente de usuários e autenticações sem degradação significativa do desempenho.

3. **Usabilidade**
   - O sistema deve ter uma interface intuitiva para facilitar o cadastro, login, e recuperação de senha.

## Casos de Uso

1. **Cadastro de Usuário**
   - **Ator:** Novo usuário
   - **Descrição:** O novo usuário fornece um e-mail e uma senha para criar uma nova conta. O sistema valida e armazena os dados.

2. **Login de Usuário**
   - **Ator:** Usuário registrado
   - **Descrição:** O usuário fornece e-mail e senha. O sistema valida as credenciais e permite o acesso ao sistema.

3. **Recuperação de Senha**
   - **Ator:** Usuário que esqueceu a senha
   - **Descrição:** O usuário solicita a recuperação de senha e recebe um link para redefinir a senha por e-mail.

4. **Logout de Usuário**
   - **Ator:** Usuário autenticado
   - **Descrição:** O usuário escolhe fazer logout. O sistema encerra a sessão ativa.

## Requisitos de Segurança

1. **Criptografia**
   - As senhas devem ser armazenadas usando hashing seguro (por exemplo, bcrypt).

2. **Proteção contra Ataques**
   - O sistema deve implementar medidas para proteger contra ataques de força bruta, como limitação de tentativas de login.

3. **Validação de Dados**
   - O sistema deve validar todos os dados de entrada para prevenir injeções e ataques similares.

4. **Autorização**
   - O sistema deve garantir que os usuários só possam acessar recursos e dados aos quais têm permissão.

## Requisitos de Interface

1. **Interface de Cadastro**
   - Campos obrigatórios: e-mail, senha
   - Validação de e-mail e força da senha

2. **Interface de Login**
   - Campos obrigatórios: e-mail, senha

3. **Interface de Recuperação de Senha**
   - Campo obrigatório: e-mail

4. **Interface de Logout**
   - Botão de logout acessível em todas as páginas enquanto o usuário estiver autenticado

## Considerações Finais

Este documento fornece uma visão geral dos requisitos para o sistema de autenticação de usuários. A implementação deve seguir estas diretrizes para garantir a segurança e a eficiência do sistema. Revisões e ajustes podem ser necessários conforme o desenvolvimento avança e novos requisitos surgem.

---

Para mais informações ou para discutir os requisitos em detalhes, entre em contato com a equipe de desenvolvimento.
