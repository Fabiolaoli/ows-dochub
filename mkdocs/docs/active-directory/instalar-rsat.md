# Instalação/Ativação do Active Directory (RSAT)

Instalação e validação das ferramentas RSAT (Remote Server Administration Tools), necessárias para administração do Active Directory em ambientes Windows corporativos. As etapas incluem a instalação do recurso via PowerShell e a validação do acesso ao console do Active Directory.

## Instalação do RSAT – Active Directory

### Abrir o PowerShell como Administrador

1. Acessar o Menu Iniciar.
2. Digitar "PowerShell" na barra de pesquisa.
3. Clicar com o botão direito sobre **Windows PowerShell**.
4. Selecionar a opção "Executar como administrador".

### Verificação dos Recursos Disponíveis

Executar o comando abaixo para listar os recursos RSAT disponíveis no sistema:

```powershell
Get-WindowsCapability -Name RSAT* -Online
```

### Instalação do Active Directory (RSAT)

Executar o comando abaixo para instalar as ferramentas do Active Directory:

```powershell
Add-WindowsCapability -Online -Name Rsat.ActiveDirectory.DS-LDS.Tools~~~~0.0.1.0
```

### Validação da Instalação

Após a instalação, executar o comando abaixo para validar o status do recurso instalado:

```powershell
Get-WindowsCapability -Name Rsat.ActiveDirectory.DS-LDS.Tools* -Online
```

Confirmar se o campo **State** apresenta o status: `Installed`.

## Acesso ao Active Directory

1. Pressionar as teclas `Win + R` para abrir o menu Executar.
2. Digitar o comando: `dsa.msc`
3. Pressionar Enter para abrir o console do Active Directory Users and Computers.
