# Atividade Avaliativa — Testes Smoke, Sanidade e Regressão

## Cenário

Uma nova versão de um sistema bancário foi implantada com:

* Correção no processo de login;
* Ajuste na exibição do saldo na tela inicial.

O objetivo dos testes é verificar se as principais funcionalidades do sistema continuam disponíveis, se as correções realizadas funcionam corretamente e se as alterações não causaram problemas em outras partes do sistema.

---

# 1. Testes Smoke

Os **testes Smoke** são realizados para verificar se as funcionalidades principais do sistema estão funcionando e se a nova versão está estável o suficiente para continuar com testes mais detalhados.

## Cenário Smoke 1 — Acessar a tela de login

**Objetivo:** Verificar se a tela de login é carregada corretamente.

**Passos:**

1. Abrir o sistema bancário;
2. Aguardar o carregamento da página inicial.

**Resultado esperado:**

A tela de login deve ser exibida corretamente, apresentando os campos de usuário, senha e o botão **Entrar**.

**Justificativa:**

Este é um teste Smoke porque verifica se uma funcionalidade essencial do sistema está disponível após a implantação da nova versão.

---

## Cenário Smoke 2 — Realizar login com credenciais válidas

**Objetivo:** Verificar se o usuário consegue acessar sua conta.

**Passos:**

1. Informar um usuário válido;
2. Informar uma senha válida;
3. Clicar no botão **Entrar**.

**Resultado esperado:**

O sistema deve autenticar o usuário e direcioná-lo para a tela inicial da conta.

**Justificativa:**

Este é um teste Smoke porque o login é uma funcionalidade crítica. Se o usuário não conseguir entrar na conta, outras funcionalidades não poderão ser utilizadas.

---

## Cenário Smoke 3 — Exibir a tela inicial da conta

**Objetivo:** Verificar se a tela inicial é apresentada após o login.

**Passos:**

1. Realizar o login com credenciais válidas;
2. Aguardar o carregamento da tela inicial.

**Resultado esperado:**

A tela inicial da conta deve ser carregada sem erros.

**Justificativa:**

Este é um teste Smoke porque verifica se o sistema consegue apresentar a área principal após a autenticação.

---

## Cenário Smoke 4 — Verificar a exibição do saldo

**Objetivo:** Verificar se a informação do saldo está disponível na tela inicial.

**Passos:**

1. Realizar o login;
2. Acessar a tela inicial;
3. Localizar a área de exibição do saldo.

**Resultado esperado:**

O saldo deve ser apresentado na tela inicial da conta.

**Justificativa:**

Este é um teste Smoke porque a visualização do saldo é uma das funcionalidades principais do sistema bancário.

---

## Cenário Smoke 5 — Verificar o acesso às principais funcionalidades

**Objetivo:** Verificar se o usuário consegue acessar as principais opções da conta.

**Passos:**

1. Realizar o login;
2. Acessar a tela inicial;
3. Verificar se as opções principais estão disponíveis.

**Resultado esperado:**

As opções principais do sistema devem estar visíveis e disponíveis para utilização.

**Justificativa:**

Este é um teste Smoke porque confirma que as funcionalidades básicas continuam acessíveis após a implantação da nova versão.

---

# 2. Testes de Sanidade

Os **testes de Sanidade** verificam especificamente se as correções e os ajustes realizados na nova versão funcionam conforme o esperado.

## Cenário de Sanidade 1 — Validar a correção do login

**Objetivo:** Verificar se o problema corrigido no login não ocorre mais.

**Passos:**

1. Acessar a tela de login;
2. Informar um usuário válido;
3. Informar uma senha válida;
4. Clicar no botão **Entrar**.

**Resultado esperado:**

O usuário deve conseguir acessar a conta sem apresentar o erro existente na versão anterior.

**Justificativa:**

Este é um teste de Sanidade porque verifica diretamente uma correção realizada na nova versão.

---

## Cenário de Sanidade 2 — Validar o login com senha incorreta

**Objetivo:** Verificar se o sistema continua tratando corretamente uma tentativa de login inválida.

**Passos:**

1. Informar um usuário válido;
2. Informar uma senha incorreta;
3. Clicar no botão **Entrar**.

**Resultado esperado:**

O sistema deve impedir o acesso e apresentar uma mensagem informando que as credenciais são inválidas.

**Justificativa:**

Este é um teste de Sanidade porque verifica se a alteração no login não causou problemas no comportamento relacionado às credenciais incorretas.

---

## Cenário de Sanidade 3 — Validar a exibição correta do saldo

**Objetivo:** Verificar se o ajuste realizado na tela inicial corrigiu a apresentação do saldo.

**Passos:**

1. Realizar o login;
2. Acessar a tela inicial;
3. Consultar o saldo apresentado.

**Resultado esperado:**

O saldo deve ser exibido corretamente, de forma clara e sem erros de visualização.

**Justificativa:**

Este é um teste de Sanidade porque valida diretamente o ajuste realizado na exibição do saldo.

---

## Cenário de Sanidade 4 — Verificar a atualização do saldo após novo acesso

**Objetivo:** Verificar se o saldo continua sendo apresentado corretamente após sair e entrar novamente no sistema.

**Passos:**

1. Realizar o login;
2. Visualizar o saldo;
3. Sair da conta;
4. Realizar o login novamente;
5. Verificar o saldo.

**Resultado esperado:**

O saldo deve continuar sendo exibido corretamente após o novo acesso.

**Justificativa:**

Este é um teste de Sanidade porque verifica se o ajuste na exibição do saldo funciona de forma consistente após uma nova autenticação.

---

## Cenário de Sanidade 5 — Verificar o carregamento da tela inicial após o login

**Objetivo:** Verificar se a correção do login permite o carregamento correto da tela inicial.

**Passos:**

1. Informar credenciais válidas;
2. Clicar em **Entrar**;
3. Aguardar o carregamento da tela inicial.

**Resultado esperado:**

A tela inicial deve ser carregada corretamente e apresentar as informações da conta, incluindo o saldo.

**Justificativa:**

Este é um teste de Sanidade porque verifica a integração direta entre a correção do login e o ajuste realizado na tela inicial.

---

# 3. Testes de Regressão

Os **testes de Regressão** verificam se as alterações realizadas na nova versão não causaram falhas em funcionalidades que já funcionavam anteriormente.

## Cenário de Regressão 1 — Realizar logout

**Objetivo:** Verificar se o usuário continua conseguindo sair da conta.

**Passos:**

1. Realizar o login;
2. Acessar a tela inicial;
3. Clicar na opção **Sair**.

**Resultado esperado:**

O sistema deve encerrar a sessão e direcionar o usuário para a tela de login.

**Justificativa:**

Este é um teste de Regressão porque verifica se uma funcionalidade existente continua funcionando após as alterações no login e na tela inicial.

---

## Cenário de Regressão 2 — Acessar os dados da conta

**Objetivo:** Verificar se as informações da conta continuam disponíveis.

**Passos:**

1. Realizar o login;
2. Acessar a opção **Dados da Conta**.

**Resultado esperado:**

O sistema deve apresentar corretamente as informações cadastradas da conta.

**Justificativa:**

Este é um teste de Regressão porque verifica se as alterações realizadas não afetaram o acesso às informações da conta.

---

## Cenário de Regressão 3 — Acessar o extrato bancário

**Objetivo:** Verificar se a funcionalidade de consulta ao extrato continua funcionando.

**Passos:**

1. Realizar o login;
2. Acessar a opção **Extrato**.

**Resultado esperado:**

O sistema deve apresentar as movimentações da conta.

**Justificativa:**

Este é um teste de Regressão porque verifica se uma funcionalidade já existente não foi afetada pelas mudanças na nova versão.

---

## Cenário de Regressão 4 — Realizar uma transferência

**Objetivo:** Verificar se a funcionalidade de transferência continua disponível.

**Passos:**

1. Realizar o login;
2. Acessar a opção **Transferência**;
3. Informar os dados necessários;
4. Confirmar a operação.

**Resultado esperado:**

O sistema deve processar a transferência e apresentar uma confirmação da operação.

**Justificativa:**

Este é um teste de Regressão porque verifica se uma funcionalidade importante do sistema continua funcionando após a implantação da nova versão.

---

## Cenário de Regressão 5 — Acessar o histórico de transações

**Objetivo:** Verificar se o usuário continua conseguindo consultar as transações realizadas.

**Passos:**

1. Realizar o login;
2. Acessar a opção **Histórico de Transações**.

**Resultado esperado:**

O sistema deve apresentar corretamente o histórico das transações da conta.

**Justificativa:**

Este é um teste de Regressão porque verifica se as alterações no login e na tela inicial não causaram impactos em funcionalidades já existentes.

---

# Comparação entre os Tipos de Teste

| Tipo de teste | Principal objetivo                                                        | Aplicação no cenário                                                 |
| ------------- | ------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| **Smoke**     | Verificar se as funcionalidades principais estão disponíveis              | Verificar login, acesso à conta e visualização do saldo              |
| **Sanidade**  | Verificar se uma correção ou alteração específica funciona                | Validar a correção do login e o ajuste na exibição do saldo          |
| **Regressão** | Verificar se alterações não causaram falhas em funcionalidades existentes | Testar logout, extrato, transferência e outras funções já existentes |

# Conclusão

Os testes Smoke, Sanidade e Regressão possuem objetivos diferentes e são importantes durante a validação de uma nova versão do sistema.

Os **testes Smoke** verificam se as principais funcionalidades estão disponíveis. Os **testes de Sanidade** validam diretamente as correções e os ajustes realizados. Já os **testes de Regressão** verificam se as mudanças não causaram problemas em funcionalidades que já funcionavam anteriormente.
