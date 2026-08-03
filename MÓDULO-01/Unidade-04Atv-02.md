# Atividade Avaliativa — Testes de Sistema e Testes de Aceitação

## Etapa 1 — Compreensão do Cenário

### Cenário

Um sistema bancário permite que usuários realizem login, acessem sua conta e visualizem seu saldo atual.

### Funcionalidades envolvidas

* Realizar login;
* Validar usuário e senha;
* Acessar a conta bancária;
* Visualizar o saldo atual;
* Exibir mensagens de erro.

### Fluxo principal

1. O usuário acessa a tela de login;
2. Informa um usuário válido;
3. Informa uma senha válida;
4. Clica no botão **Entrar**;
5. O sistema valida as informações;
6. O usuário acessa a conta;
7. O saldo atual é exibido.

### Variações de fluxo

* O usuário informa uma senha incorreta;
* O usuário informa um usuário inexistente;
* O usuário deixa os campos vazios;
* O sistema apresenta uma mensagem de erro;
* O acesso à conta é bloqueado.

---

# Etapa 2 — Testes de Sistema

## Teste de Sistema — Fluxo Principal 1

| Campo                  | Descrição                                                                                                                  |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **ID**                 | TS-001                                                                                                                     |
| **Título**             | Realizar login com credenciais válidas                                                                                     |
| **Pré-condições**      | O usuário possui uma conta ativa e cadastrada.                                                                             |
| **Passos**             | 1. Acessar a tela de login.<br>2. Informar um usuário válido.<br>3. Informar uma senha válida.<br>4. Clicar em **Entrar**. |
| **Resultado esperado** | O sistema deve validar as informações e direcionar o usuário para a tela da conta.                                         |

## Teste de Sistema — Fluxo Principal 2

| Campo                  | Descrição                                                                               |
| ---------------------- | --------------------------------------------------------------------------------------- |
| **ID**                 | TS-002                                                                                  |
| **Título**             | Visualizar o saldo após realizar o login                                                |
| **Pré-condições**      | O usuário possui uma conta ativa e está conectado ao sistema.                           |
| **Passos**             | 1. Realizar o login.<br>2. Acessar a tela principal da conta.<br>3. Visualizar o saldo. |
| **Resultado esperado** | O sistema deve apresentar o saldo atual na tela da conta.                               |

## Teste de Sistema — Fluxo Alternativo 1

| Campo                  | Descrição                                                                                                                     |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **ID**                 | TS-003                                                                                                                        |
| **Título**             | Tentar realizar login com senha incorreta                                                                                     |
| **Pré-condições**      | O usuário possui uma conta cadastrada.                                                                                        |
| **Passos**             | 1. Acessar a tela de login.<br>2. Informar um usuário válido.<br>3. Informar uma senha incorreta.<br>4. Clicar em **Entrar**. |
| **Resultado esperado** | O sistema deve impedir o acesso e apresentar uma mensagem informando que as credenciais são inválidas.                        |

## Teste de Sistema — Fluxo Alternativo 2

| Campo                  | Descrição                                                                          |
| ---------------------- | ---------------------------------------------------------------------------------- |
| **ID**                 | TS-004                                                                             |
| **Título**             | Tentar realizar login sem preencher os campos                                      |
| **Pré-condições**      | O usuário está na tela de login.                                                   |
| **Passos**             | 1. Deixar os campos de usuário e senha vazios.<br>2. Clicar em **Entrar**.         |
| **Resultado esperado** | O sistema deve informar que os campos são obrigatórios e impedir o acesso à conta. |

---

# Etapa 3 — Testes de Aceitação

## Teste de Aceitação — Fluxo Principal 1

| Campo                  | Descrição                                                                                          |
| ---------------------- | -------------------------------------------------------------------------------------------------- |
| **ID**                 | TA-001                                                                                             |
| **Título**             | Acessar a conta bancária com sucesso                                                               |
| **Pré-condições**      | O cliente possui uma conta ativa e credenciais válidas.                                            |
| **Passos**             | 1. Acessar o sistema bancário.<br>2. Informar as credenciais corretas.<br>3. Clicar em **Entrar**. |
| **Resultado esperado** | O cliente deve conseguir acessar sua conta e visualizar suas informações.                          |

## Teste de Aceitação — Fluxo Principal 2

| Campo                  | Descrição                                                                                                |
| ---------------------- | -------------------------------------------------------------------------------------------------------- |
| **ID**                 | TA-002                                                                                                   |
| **Título**             | Consultar o saldo atual da conta                                                                         |
| **Pré-condições**      | O cliente possui uma conta ativa e está conectado.                                                       |
| **Passos**             | 1. Realizar o login.<br>2. Acessar a tela principal.<br>3. Consultar o saldo.                            |
| **Resultado esperado** | O cliente deve visualizar seu saldo atual de forma clara e conseguir acompanhar sua situação financeira. |

## Teste de Aceitação — Fluxo Alternativo 1

| Campo                  | Descrição                                                                                                      |
| ---------------------- | -------------------------------------------------------------------------------------------------------------- |
| **ID**                 | TA-003                                                                                                         |
| **Título**             | Receber uma mensagem ao informar senha incorreta                                                               |
| **Pré-condições**      | O cliente possui uma conta cadastrada.                                                                         |
| **Passos**             | 1. Informar o usuário correto.<br>2. Informar uma senha incorreta.<br>3. Clicar em **Entrar**.                 |
| **Resultado esperado** | O cliente não deve acessar a conta e deve receber uma mensagem clara informando que o login não foi realizado. |

## Teste de Aceitação — Fluxo Alternativo 2

| Campo                  | Descrição                                                                                          |
| ---------------------- | -------------------------------------------------------------------------------------------------- |
| **ID**                 | TA-004                                                                                             |
| **Título**             | Receber orientação ao deixar os campos vazios                                                      |
| **Pré-condições**      | O cliente está na tela de login.                                                                   |
| **Passos**             | 1. Deixar os campos vazios.<br>2. Clicar em **Entrar**.                                            |
| **Resultado esperado** | O cliente deve receber uma mensagem informando que precisa preencher os campos antes de continuar. |

---

# Etapa 4 — Justificativa e Classificação

## Justificativas dos Testes de Sistema

### TS-001 — Login com credenciais válidas

Este é um teste de sistema porque verifica o funcionamento integrado da tela de login, da validação das credenciais e do acesso à tela da conta.

* **Objetivo:** Verificar se o login funciona corretamente;
* **Ponto de vista:** Funcionamento técnico e funcional do sistema;
* **Validação:** Integração entre a tela de login e a tela da conta.

### TS-002 — Visualizar o saldo

Este é um teste de sistema porque verifica a integração entre o login, o acesso à conta e a exibição do saldo.

* **Objetivo:** Verificar se o saldo é apresentado corretamente;
* **Ponto de vista:** Funcionamento do sistema;
* **Validação:** Integração entre a conta e a funcionalidade de consulta de saldo.

### TS-003 — Login com senha incorreta

Este é um teste de sistema porque verifica como o sistema responde a uma tentativa de login inválida.

* **Objetivo:** Verificar se o acesso é bloqueado;
* **Ponto de vista:** Comportamento funcional do sistema;
* **Validação:** Exibição da mensagem de erro e bloqueio do acesso.

### TS-004 — Login com campos vazios

Este é um teste de sistema porque verifica o comportamento da tela de login quando as informações obrigatórias não são preenchidas.

* **Objetivo:** Verificar a validação dos campos;
* **Ponto de vista:** Funcionamento do sistema;
* **Validação:** Mensagens de erro e bloqueio do acesso.

## Justificativas dos Testes de Aceitação

### TA-001 — Acessar a conta bancária

Este é um teste de aceitação porque verifica se o cliente consegue acessar sua conta, atendendo à necessidade esperada pelo negócio.

* **Objetivo:** Permitir que o cliente acesse sua conta;
* **Ponto de vista:** Cliente e negócio;
* **Validação:** Valor entregue ao usuário.

### TA-002 — Consultar o saldo

Este é um teste de aceitação porque verifica se o cliente consegue visualizar sua situação financeira.

* **Objetivo:** Permitir a consulta do saldo;
* **Ponto de vista:** Cliente;
* **Validação:** Utilidade e valor entregue ao usuário.

### TA-003 — Mensagem de senha incorreta

Este é um teste de aceitação porque verifica se o cliente recebe uma orientação clara quando não consegue acessar a conta.

* **Objetivo:** Informar o problema ao cliente;
* **Ponto de vista:** Cliente;
* **Validação:** Clareza da comunicação e segurança do acesso.

### TA-004 — Mensagem para campos vazios

Este é um teste de aceitação porque verifica se o cliente recebe orientação para preencher as informações necessárias.

* **Objetivo:** Orientar o cliente durante o login;
* **Ponto de vista:** Cliente;
* **Validação:** Facilidade de uso e clareza das mensagens.

---

# Etapa 5 — Revisão por Pares

Durante a revisão dos testes criados por outros alunos, devem ser verificados:

| Critério               | Verificação                                                                  |
| ---------------------- | ---------------------------------------------------------------------------- |
| **Clareza**            | Os casos de teste estão escritos de forma compreensível?                     |
| **Estrutura**          | Todos os campos obrigatórios foram preenchidos?                              |
| **Coerência**          | O teste foi classificado corretamente como teste de sistema ou de aceitação? |
| **Resultado esperado** | O resultado esperado está claro e pode ser verificado?                       |

## Conclusão

Os testes de sistema verificam o funcionamento e a integração das funcionalidades do sistema. Os testes de aceitação verificam se o sistema atende às necessidades do usuário e entrega o valor esperado pelo negócio.
