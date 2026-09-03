# Criação de usuário no Active Directory (AD)

Criação de usuários no Active Directory (AD), incluindo definição de login, configuração de grupos de acesso, associação organizacional e vinculação do gestor responsável. O processo garante a padronização dos acessos corporativos e a correta integração do colaborador ao ambiente da empresa.

## Identificação das Informações do Colaborador

Localizar no chamado as seguintes informações do colaborador:

- Nome completo
- Departamento/área de atuação

## Criação do Usuário no AD

1. Acessar o Active Directory.
2. Navegar até a pasta correspondente ao departamento do colaborador.
3. Selecionar a pasta **Users**.
4. Clicar com o botão direito na área em branco.
5. Selecionar: **New > User**.

## Padrão de Cadastro

### E-mail Corporativo

Definir o e-mail no seguinte padrão:

```
primeironome.ultimonome@olos.com.br
```

### Login de Rede

Definir o login utilizando:

- 3 primeiras letras do primeiro nome
- 3 primeiras letras do sobrenome

Exemplo: `joasil`

## Configurações do Usuário

### Aba "General"

Preencher o nome completo do colaborador.

### Aba "Member Of"

Adicionar os seguintes grupos de acesso:

- G_fsso
- G_VPN
- Wifi

## Configurações Organizacionais

- **Empresa**: definir a empresa como `OLOS`.
- **Caixa Postal**: configurar a caixa postal como `O365`.
- **Organização**: definir o **Manager** (gestor responsável pelo colaborador).
