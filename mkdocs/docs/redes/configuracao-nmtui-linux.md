# Configuração de Rede no Linux via NMTUI

Configurar a conexão de rede no terminal Linux utilizando o `nmtui` e, após validar a conectividade, abrir a página de monitoramento em tela cheia para acompanhamento contínuo do ambiente.

## Acessar o terminal TTY

Pressione as teclas `CTRL + ALT + F1`. Isso abrirá o terminal de configuração do sistema.

## Abrir o gerenciador de rede

Execute o comando:

```bash
sudo nmtui
```

O `nmtui` é a interface gráfica em modo texto utilizada para gerenciamento de rede no Linux.

## Configurar a conexão

No menu do `nmtui`:

1. Selecione "Editar uma conexão".
2. Localize e selecione a conexão.
3. Configure os parâmetros necessários da rede.
4. Salve as alterações realizadas.

## Ativar a conexão configurada

Ainda no `nmtui`:

1. Volte ao menu principal.
2. Selecione "Ativar uma conexão".
3. Ative a conexão configurada anteriormente.

## Sair do NMTUI

Selecione: **Sair**.

## Testar conectividade

No terminal, execute o comando:

```bash
ping 8.8.8.8
```

Se houver resposta do ping, a conexão estará funcionando corretamente. Para interromper o teste, pressione `CTRL + C`.

## Retornar para a interface gráfica

Pressione `CTRL + ALT + F7`. Isso retornará ao ambiente gráfico do sistema.

## Abrir página de monitoramento

Abra o navegador e acesse `uptime.olos.com.br`. Depois pressione `F11` para colocar o navegador em modo tela cheia.

## Resultado Esperado

- Rede configurada e conectada com sucesso
- Comunicação validada via ping
- Página de monitoramento aberta em fullscreen para acompanhamento contínuo do ambiente
