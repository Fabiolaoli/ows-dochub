# Colocar o Usuário como ADMIN

Inclusão de um colaborador no grupo de administradores locais da máquina e no grupo de administradores do domínio, utilizando o Active Directory e o gerenciamento local do Windows 11.

## Inclusão no Grupo de Administradores Locais

1. Realizar o login na máquina do colaborador utilizando a conta administrativa local: `.\admin`
2. Pesquisar por **Gerenciamento do Computador** e abrir a ferramenta.
3. Acessar:
   - Ferramentas do Sistema
   - Usuários e Grupos Locais
   - Grupos
4. Abrir o grupo **Administradores**.
5. Clicar em **Adicionar**.
6. Inserir o usuário do colaborador.

   > **Importante:** A VPN deve estar conectada para que o usuário seja localizado corretamente.

7. Clicar em **Aplicar**.
8. Finalizar clicando em **OK**.

## Inclusão no Grupo Administrators via Active Directory

1. Acessar o Active Directory pela máquina administrativa.
2. Localizar o usuário do colaborador.
3. Abrir as propriedades do usuário.
4. Acessar a aba **Membro de**.
5. Clicar em **Adicionar**.
6. Inserir o nome: `admin`
7. Clicar em **Verificar Nomes**.
8. Selecionar o grupo **Administrators**.
9. Clicar em **OK**.
10. Finalizar clicando em **Aplicar** e depois em **OK**.
