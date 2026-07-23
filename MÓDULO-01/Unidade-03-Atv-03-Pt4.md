# Exercício 4 — Testes de Sistema

## Objetivo

Realizar testes de sistema por meio da interface da aplicação **Clínica Psi**, simulando fluxos executados pelo usuário final.

**Sistema utilizado:**  
https://andrelbribeiro.github.io/clinica-psi/

---

# Cenário A — Atendimento Completo

## Pré-condições
- Sistema disponível.
- Usuário autenticado.
- Não existir paciente com o mesmo CPF.

## Dados utilizados

| Campo | Valor |
|--------|-------|
| Nome | Maria da Silva |
| CPF | 123.456.789-00 |
| Psicólogo | João Pereira |
| Data | 25/07/2026 |
| Horário | 09:00 |

## Passos

1. Cadastrar um paciente.
2. Localizar o paciente pela pesquisa.
3. Realizar um agendamento.
4. Fazer o check-in.
5. Registrar a evolução da sessão.
6. Lançar a receita.
7. Conferir o relatório financeiro.

## Resultado esperado

- Paciente cadastrado com sucesso.
- Pesquisa retorna o paciente.
- Agendamento criado.
- Check-in realizado.
- Evolução registrada.
- Receita salva.
- Atendimento aparece no relatório financeiro.

## Resultado obtido

Todos os passos foram executados corretamente pelo sistema.

## Situação

**Aprovado**

## Evidência

Capturas de tela do cadastro, agendamento, check-in, evolução, receita e relatório financeiro.

## Justificativa

O sistema executou todo o fluxo de atendimento sem apresentar erros.

---

# Cenário B — Reagendamento

## Pré-condições

- Paciente cadastrado.
- Consulta previamente agendada.

## Dados utilizados

| Campo | Valor |
|--------|-------|
| Paciente | Maria da Silva |
| Horário anterior | 25/07/2026 - 09:00 |
| Novo horário | 25/07/2026 - 10:00 |

## Passos

1. Criar um agendamento.
2. Reagendar a consulta.
3. Verificar a liberação do horário anterior.
4. Verificar a ocupação do novo horário.
5. Conferir os dados apresentados na agenda.

## Resultado esperado

- Consulta reagendada.
- Horário antigo disponível novamente.
- Novo horário ocupado.
- Agenda atualizada corretamente.

## Resultado obtido

O reagendamento foi realizado conforme esperado.

## Situação

**Aprovado**

## Evidência

Capturas de tela da agenda antes e depois do reagendamento.

## Justificativa

A agenda foi atualizada corretamente e os horários refletiram a alteração.

---

# Cenário C — Controle de Estoque

## Pré-condições

- Usuário com permissão para gerenciar estoque.

## Dados utilizados

| Campo | Valor |
|--------|-------|
| Produto | Luvas descartáveis |
| Entrada | 100 unidades |
| Saída | 20 unidades |
| Estoque mínimo | 30 unidades |

## Passos

1. Cadastrar um produto.
2. Registrar uma entrada.
3. Registrar uma saída.
4. Verificar a quantidade final.
5. Verificar o alerta de estoque mínimo.

## Resultado esperado

- Produto cadastrado.
- Entrada registrada.
- Saída registrada.
- Estoque final igual a 80 unidades.
- Alerta exibido apenas quando atingir o estoque mínimo.

## Resultado obtido

O sistema atualizou corretamente a quantidade disponível.

## Situação

**Aprovado**

## Evidência

Capturas de tela do cadastro do produto e da movimentação de estoque.

## Justificativa

O sistema realizou corretamente os cálculos e atualizou o estoque.

---

# Cenário D — Controle de Acesso

## Pré-condições

- Existirem dois usuários cadastrados:
  - Recepcionista.
  - Psicólogo.

## Dados utilizados

| Perfil | Permissão |
|---------|-----------|
| Recepcionista | Agenda e cadastro |
| Psicólogo | Agenda, prontuário e evolução |

## Passos

1. Criar perfis com diferentes permissões.
2. Entrar como recepcionista.
3. Tentar acessar prontuários.
4. Entrar como psicólogo.
5. Verificar se o acesso autorizado funciona.

## Resultado esperado

- Recepcionista não acessa prontuários.
- Psicólogo acessa normalmente.
- Sistema respeita as permissões dos perfis.

## Resultado obtido

As permissões foram aplicadas conforme esperado.

## Situação

**Aprovado**

## Evidência

Capturas de tela dos acessos com cada perfil.

## Justificativa

O controle de acesso protegeu corretamente as funcionalidades restritas.

---

# Conclusão

Os testes de sistema permitiram validar os principais fluxos da aplicação Clínica Psi por meio da interface do usuário. Em todos os cenários executados, o sistema apresentou o comportamento esperado, atendendo aos requisitos funcionais avaliados. Os resultados obtidos demonstram que as funcionalidades testadas estão operando corretamente e oferecem suporte adequado às atividades da clínica.
