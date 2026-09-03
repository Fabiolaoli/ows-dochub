# Resolução de problemas de rede no Linux

Resolução de problemas de rede em sistemas Linux, realizando ações como reinicialização de serviços de rede, renovação de IP e limpeza de cache DNS.

## Abrir o Terminal

Utilize o atalho `Ctrl + Alt + T` ou pesquise por **Terminal** no menu de aplicativos.

## Comandos Principais

### Reiniciar Serviço de Rede

Reinicia os serviços responsáveis pelas conexões de rede no Linux.

```bash
sudo systemctl restart NetworkManager
```

Em algumas distribuições Linux, o serviço pode variar.

### Reiniciar Configurações TCP/IP

Renova as configurações de rede da interface.

#### Liberar IP Atual

```bash
sudo dhclient -r
```

Libera o endereço IP atual da máquina.

#### Renovar Endereço IP

```bash
sudo dhclient
```

Solicita um novo endereço IP ao servidor DHCP da rede.

## Comandos Adicionais

### Limpar Cache DNS

Para distribuições utilizando `systemd-resolved`:

```bash
sudo systemd-resolve --flush-caches
```

ou

```bash
sudo resolvectl flush-caches
```

Limpa o cache DNS armazenado localmente.

### Reiniciar Serviço DNS

Caso o problema persista:

```bash
sudo systemctl restart systemd-resolved
```

Reinicia o serviço de resolução DNS.

## Verificar Configurações de Rede

### Verificar Endereço IP

```bash
ip addr
```

Exibe as interfaces de rede e endereços IP configurados.

### Testar Conectividade

```bash
ping 8.8.8.8
```

Testa a comunicação com a internet utilizando o DNS público do Google.

> **Observação:** Alguns comandos podem variar dependendo da distribuição Linux utilizada, como Ubuntu, Debian, Fedora ou CentOS.
