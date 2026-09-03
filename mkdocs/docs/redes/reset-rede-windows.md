# Máquina não reconhece as SSID

Redefinição das configurações de rede no Windows 11, auxiliando na correção de falhas de conexão, DNS e obtenção de endereço IP.

## Procedimento

1. Abrir o menu Iniciar.
2. Pesquisar por **CMD**.
3. Executar o Prompt de Comando como administrador.
4. Utilizar os comandos abaixo conforme a necessidade.

## Comandos Principais

### Reset do Winsock

```cmd
netsh winsock reset
```

Reinicia o catálogo Winsock, responsável pelo gerenciamento das conexões de rede do Windows.

### Reset do TCP/IP

```cmd
netsh int ip reset
```

Redefine o protocolo TCP/IP, conjunto fundamental de comunicação utilizado em redes e conexões com a internet.

## Comandos Adicionais

Caso os comandos anteriores não resolvam o problema, executar os comandos abaixo:

### Liberar o IP Atual

```cmd
ipconfig /release
```

Libera o endereço IP atualmente atribuído à máquina.

### Renovar o Endereço IP

```cmd
ipconfig /renew
```

Solicita um novo endereço IP ao servidor de rede.

### Limpar Cache DNS

```cmd
ipconfig /flushdns
```

Limpa o cache DNS armazenado localmente, auxiliando na resolução de problemas de navegação e acesso a sites.
