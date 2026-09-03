# Notebook Não Espelha no Monitor

Este procedimento deve ser realizado quando o notebook não estiver espelhando imagem no monitor externo, mesmo após a validação das atualizações do sistema. O objetivo é verificar as configurações de vídeo na BIOS e, se necessário, atualizar o driver gráfico no Windows.

## Validar Atualizações do Sistema

Antes de iniciar as configurações da BIOS, verificar se todas as atualizações do Windows e drivers estão instaladas corretamente.

## Verificar Configurações da BIOS

### Acessar a BIOS

1. Reiniciar o notebook.
2. Durante a inicialização, pressionar repetidamente a tecla `F2` até entrar na BIOS.

### Caminho das Configurações de Vídeo

No Dell Latitude 3450, procurar por opções como:

- Vídeo ou Display

### Configurações da GPU

Verificar se aparecem opções como:

- Switchable Graphics
- Hybrid Graphics
- Enable Graphics Device

### Configuração Correta

As opções devem estar configuradas como **Enabled** ou **ON**.

Caso existam opções de GPU, podem aparecer:

- UMA Only
- Discrete
- Hybrid

Selecionar: **Hybrid** ou **Switchable**.

### Salvar Alterações

Após ajustar as configurações:

1. Clicar em **Apply**.
2. Depois em **Exit** ou pressionar a tecla `F10` para salvar e sair.

## Atualizar Driver de Vídeo no Windows

Se as configurações estiverem corretas e o problema persistir:

1. Pressionar `Windows + X`.
2. Acessar **Gerenciamento do Computador**.
3. Ir em **Adaptadores de Vídeo**.
4. Selecionar **Intel(R) UHD Graphics**.
5. Ir na aba **Driver**.
6. Clicar em **Atualizar Driver**.
7. Finalizar a atualização e reiniciar o equipamento, se necessário.
