# Atividade Avaliativa – Testes Funcionais

## Sistema Fictício: Loja Virtual

O sistema permite que o cliente:
- Realize cadastro e login;
- Pesquise produtos;
- Adicione produtos ao carrinho;
- Finalize a compra com cartão de crédito;
- Receba um e-mail de confirmação do pedido.

## Testes Unitários

**Objetivo:** Verificar o funcionamento de pequenas partes do sistema de forma isolada.

**Exemplos:**
- Validar o cálculo do valor total do carrinho.
- Verificar a validação da senha no cadastro.
- Testar o cálculo de descontos em promoções.

**Justificativa:**
Os testes unitários analisam funções, métodos ou classes individualmente, garantindo que cada componente funcione corretamente sem depender de outros módulos.

---

## Testes de Integração

**Objetivo:** Verificar a comunicação entre diferentes módulos do sistema.

**Exemplos:**
- Testar a integração entre o login e o banco de dados.
- Verificar a comunicação entre o carrinho de compras e o sistema de pagamento.
- Confirmar a atualização do estoque após uma compra.

**Justificativa:**
Esses testes garantem que os componentes do sistema funcionem corretamente quando integrados.

---

## Testes de Sistema

**Objetivo:** Validar o funcionamento completo da aplicação.

**Exemplos:**
- Realizar uma compra completa, desde o login até a confirmação do pedido.
- Pesquisar um produto, adicioná-lo ao carrinho e finalizar a compra.
- Consultar o histórico de pedidos.

**Justificativa:**
Os testes de sistema verificam se todas as funcionalidades trabalham em conjunto conforme os requisitos do software.

---

## Testes de Aceitação

**Objetivo:** Confirmar que o sistema atende às necessidades do cliente e dos usuários finais.

**Exemplos:**
- O cliente consegue concluir uma compra sem erros.
- O administrador consegue cadastrar novos produtos.
- O usuário recebe o e-mail de confirmação após finalizar a compra.

**Justificativa:**
Os testes de aceitação validam que o sistema está pronto para uso e atende aos requisitos definidos pelo cliente.

---

# Resumo

| Tipo de Teste | Objetivo |
|----------------|----------|
| **Unitário** | Testar componentes individuais do sistema. |
| **Integração** | Verificar a comunicação entre módulos. |
| **Sistema** | Validar o funcionamento completo da aplicação. |
| **Aceitação** | Confirmar que o sistema atende aos requisitos do cliente. |
