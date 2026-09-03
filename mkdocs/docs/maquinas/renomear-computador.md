# Renomear o computador

Identificação do serial number da máquina, padronização do nome do equipamento e ingresso no domínio corporativo da empresa, garantindo a correta integração do dispositivo ao ambiente organizacional.

## Identificação do Serial Number da Máquina

1. Abrir o Prompt de Comando (CMD).
2. Executar o comando abaixo para identificar o serial number do equipamento:

   ```cmd
   wmic bios get serialnumber
   ```

## Alteração do Nome da Máquina

1. Acessar **Configurações**.
2. Selecionar **Sistema**.
3. Clicar em **Sobre**.
4. Acessar a opção **Domínio ou Grupo de Trabalho**.
5. Selecionar **Alterar**.
6. Definir o nome da máquina seguindo o padrão:

   ```
   OLOSNBK + Serial Number do equipamento
   ```

## Ingresso no Domínio Corporativo

1. Na seção **Membro de**, selecionar a opção **Domínio**.
2. Inserir o domínio corporativo:

   ```
   intra.olos.com.br
   ```

3. Clicar em **OK** para concluir o processo de ingresso no domínio.
