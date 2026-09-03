# Criptografia de Máquina

Validação e correção de falhas na ativação do BitLocker quando a criptografia não é iniciada corretamente no primeiro acesso.

## Verificação Inicial do BitLocker

1. Abrir o menu Iniciar do Windows.
2. Pesquisar por **BitLocker**.
3. Selecionar **Gerenciar BitLocker**.
4. Verificar se o BitLocker está desativado.
5. Tentar ativar manualmente.
6. Validar se o sistema retorna a mensagem: "O sistema não pode encontrar o arquivo especificado".

Caso a mensagem seja exibida, seguir com o procedimento abaixo.

## Validação de Secure Boot e TPM 2.0

### Verificação do Secure Boot

1. Pressionar `Windows + R`.
2. Digitar `msinfo32` e pressionar Enter.
3. Verificar o campo **Estado da Inicialização Segura**:
   - O status deve estar como **Ativada**.
   - Caso não esteja, continuar com o procedimento.

### Verificação do TPM

1. Pressionar `Windows + I`.
2. Acessar **Privacidade e Segurança**.
3. Selecionar **Segurança do Windows**.
4. Acessar **Segurança do Dispositivo**.
5. Selecionar **Detalhes do Processador de Segurança**.
6. Verificar o campo **Versão de especificação**:
   - Deve constar a versão **2.0**.
   - Caso não esteja, o TPM 2.0 deverá ser habilitado, se suportado pelo equipamento.
   - Caso esteja correto, prosseguir com o procedimento.

### Ativação do Secure Boot na BIOS

1. Reiniciar o computador.
2. Pressionar `F12` para acessar a BIOS.
3. Acessar **BIOS Configuration**.
4. Selecionar **Boot Option**.
5. Localizar a opção **Secure Boot** e habilitá-la.
6. Salvar as alterações.
7. Sair da BIOS.

## Validação Final da Criptografia

Após iniciar o Windows:

1. Abrir o menu Iniciar.
2. Pesquisar por **BitLocker**.
3. Selecionar **Gerenciar BitLocker**.
4. Tentar ativar manualmente novamente.
5. Verificar se a mensagem "O sistema não pode encontrar o arquivo especificado" não é mais apresentada.
6. Aguardar alguns minutos para confirmar se o processo de criptografia foi iniciado corretamente.
