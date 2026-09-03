# Sessão do ORA

Reinicialização de Sessão RDS e Reconfiguração de Máquina Remota.

Desconexão de sessões ativas no ambiente RDS e a reconfiguração da máquina remota do colaborador, utilizando o mRemoteNG e os serviços de Remote Desktop Services.

## Procedimento

1. Abrir o mRemoteNG.
2. Acessar o servidor **ORA-BROKER**.
3. Navegar até **Remote Desktop Services**.
4. Selecionar **Collections**.
5. Acessar a aba **Connections**.
6. Localizar o usuário do colaborador.
7. Selecionar a sessão ativa e clicar em **Disconnect**.
8. Atualizar a lista em **Tasks** até que o usuário não apareça mais entre as conexões ativas.
9. Após a desconexão completa, orientar o colaborador a excluir todas as máquinas remotas configuradas.
10. Solicitar que o colaborador realize o download de uma nova máquina remota através do portal:

    ```
    https://10.15.150.152/RDWeb/Pages/en-US/login.aspx?ReturnUrl=/RDWeb/Pages/en-US/Default.aspx
    ```
