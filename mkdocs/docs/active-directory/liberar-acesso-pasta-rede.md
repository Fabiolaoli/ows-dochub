# Liberação de Acesso na Pasta de Redes

Este procedimento tem como objetivo orientar a liberação de acesso a pastas compartilhadas através do Active Directory, garantindo que o colaborador receba as permissões adequadas conforme o grupo de acesso da área.

## Validação da Pasta Solicitada

1. Acessar o chamado.
2. Copiar o link da pasta solicitada.
3. Abrir o Explorador de Arquivos.
4. Colar o caminho da pasta na barra de endereço em **Início**.
5. Validar o conteúdo da pasta.

> **Observação:** Caso necessário, solicitar ao HEAD/responsável da área a aprovação para liberação do acesso.

## Verificação do Grupo de Permissão

1. Clicar com o botão direito sobre a pasta.
2. Selecionar:
   - Propriedades
   - Segurança
3. Identificar o grupo de acesso correspondente ao perfil do solicitante.
4. Validar o grupo com permissão de **Leitura e Escrita (RW)**.

## Inclusão do Usuário no Grupo de Acesso

1. Acessar o Active Directory.
2. Navegar até: `intra.olos.com.br`
3. Localizar a pasta **Group**.
4. Encontrar o grupo relacionado à pasta compartilhada.
5. Abrir o grupo identificado.
6. Acessar a aba **Membros**.
7. Clicar em **Adicionar**.
8. Inserir o nome do usuário.
9. Clicar em **Verificar Nomes**.
10. Confirmar clicando em **OK**.

> **Observação:** Após a inclusão no grupo, pode ser necessário solicitar que o colaborador realize logoff/logon para atualização das permissões.
