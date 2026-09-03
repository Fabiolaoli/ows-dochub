# Chamado de Arquivo Host

Alteração do arquivo Hosts em máquinas corporativas, utilizando acesso remoto via AnyDesk.

## Procedimento

1. Entrar em contato com o colaborador e solicitar o código de acesso do AnyDesk.
2. Conectar na máquina do colaborador.
3. Confirmar com o colaborador qual alteração deverá ser realizada no arquivo Hosts.
4. Bloquear a máquina do colaborador.
5. Realizar login com o usuário administrativo local: `.\admin`
6. Abrir o Explorador de Arquivos.
7. Navegar até o seguinte caminho: `C:\Windows\System32\drivers\e`

   > ⚠️ **Revisar:** O caminho informado no documento original está incompleto (`C:\Windows\System32\drivers\e`). O caminho padrão do arquivo hosts no Windows é `C:\Windows\System32\drivers\etc`. Confirmar antes de corrigir.

8. Localizar o arquivo `hosts`.
9. Abrir o arquivo utilizando o Bloco de Notas ou o Notepad++.
10. Realizar as alterações necessárias.
11. Salvar o arquivo após a conclusão das modificações.
