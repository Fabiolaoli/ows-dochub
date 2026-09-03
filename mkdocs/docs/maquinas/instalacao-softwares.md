# Instalação de softwares

Instalação e configuração de softwares corporativos, atualização do sistema operacional e drivers, além da validação e configuração do BitLocker em notebooks da empresa. As etapas descritas garantem a padronização, segurança e correto funcionamento dos equipamentos no ambiente corporativo.

## Acesso à Pasta de Softwares Corporativos

1. Abrir o Explorador de Arquivos.
2. No campo de pesquisa/endereço, acessar o caminho:

   ```
   \\10.15.5.30\softwares$
   ```

3. Inserir login e senha corporativos quando solicitado.

## Bitdefender

1. Acessar o seguinte caminho:

   ```
   Bitdefender > pacote notebook Windows - bitlocker > NEW > 4-08-2025 > setupdownload
   ```

2. Executar o instalador e concluir a instalação do antivírus.

## AnyDesk

1. Executar o arquivo `AnyDesk.exe`.
2. Durante a instalação, desmarcar a opção "Instalar impressora AnyDesk".
3. Após a instalação, realizar a atualização do aplicativo.

## Atualização do Sistema Operacional

### Windows Update

1. Acessar **Configurações**.
2. Acessar **Windows Update**.
3. Executar todas as atualizações disponíveis do sistema operacional.

## Atualização de Drivers

Realizar a atualização dos drivers de acordo com o fabricante do equipamento:

- **Lenovo**: acessar o portal de suporte da Lenovo.
- **Dell**: acessar a página de suporte da Dell Brasil.

## Configuração e Verificação do BitLocker

### Verificação do Status

Abrir o Prompt de Comando (CMD) e executar o comando:

```cmd
manage-bde -status
```

### Ativação do BitLocker

Caso o BitLocker não esteja ativo, abrir o PowerShell como administrador e executar o comando:

```powershell
resume-bitlocker -mountpoint "C:"
```

### Definição de Senha do Administrador

1. Acessar:

   ```
   Win + X > Gerenciamento de Computador > Usuários e Grupos Locais > Usuários
   ```

2. Localizar o usuário **Admin**.
3. Clicar com o botão direito sobre o usuário e selecionar a opção "Definir Senha".

### Correção de Solicitação de Senha do BitLocker na Inicialização

Caso o BitLocker solicite senha durante a inicialização do equipamento:

1. Acessar o diretório:

   ```
   C:\Windows\System32\Recovery
   ```

2. Recortar o arquivo localizado na pasta e colá-lo na área de trabalho.
3. Reiniciar o equipamento para validar a correção do problema.
