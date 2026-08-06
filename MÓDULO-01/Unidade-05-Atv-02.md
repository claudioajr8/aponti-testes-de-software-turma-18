# Plano de Testes — Site da Clínica de Psicologia

## 1. Objetivo do Plano de Testes

O objetivo deste plano de testes é definir como as funcionalidades do site da clínica de psicologia serão verificadas antes da entrega do projeto.

Os testes serão realizados para identificar falhas, garantir o funcionamento correto das principais funcionalidades, avaliar a facilidade de uso e reduzir riscos relacionados à segurança e à privacidade dos dados dos usuários.

Como o projeto possui prazo de entrega definido e um time reduzido, os testes serão priorizados de acordo com o risco e a importância de cada funcionalidade.

---

## 2. Escopo de Testes

Os testes serão realizados nas principais funcionalidades do site:

* Navegação entre as páginas;
* Exibição das informações sobre a clínica e os profissionais;
* Funcionamento dos menus, botões e links;
* Formulário de contato;
* Validação dos campos obrigatórios;
* Envio de mensagens;
* Agendamento de consultas, caso essa funcionalidade esteja disponível;
* Login e acesso a áreas restritas, caso existam;
* Exibição correta do site em computadores, celulares e tablets;
* Funcionamento do site nos principais navegadores.

### Funcionalidades fora do escopo

Neste momento, testes avançados de carga, estresse e capacidade não serão priorizados devido ao prazo definido e à quantidade reduzida de pessoas na equipe.

Entretanto, será realizada uma verificação básica do tempo de carregamento das páginas principais.

---

## 3. Tipos de Teste Aplicados

### Testes funcionais

Serão realizados para verificar se as funcionalidades do site funcionam conforme o esperado.

Exemplos:

* Verificar se os menus direcionam para as páginas corretas;
* Testar os botões e links;
* Preencher e enviar o formulário de contato;
* Verificar se os campos obrigatórios são validados;
* Testar o agendamento de consultas;
* Verificar o funcionamento do login, caso exista.

### Testes de usabilidade

Serão realizados para avaliar se o site é simples, organizado e fácil de utilizar.

Serão analisados:

* Facilidade para encontrar informações;
* Clareza dos textos e dos botões;
* Organização das páginas;
* Facilidade para preencher formulários;
* Compreensão das mensagens de erro;
* Facilidade para entrar em contato ou realizar um agendamento.

### Testes de compatibilidade

Serão realizados para verificar se o site funciona corretamente em diferentes dispositivos e navegadores.

Serão utilizados:

* Computadores;
* Celulares;
* Tablets;
* Google Chrome;
* Microsoft Edge;
* Mozilla Firefox.

### Testes de segurança

Serão realizados testes básicos para verificar:

* Proteção das informações enviadas pelos usuários;
* Validação dos dados inseridos nos formulários;
* Controle de acesso às áreas restritas;
* Proteção do login, caso exista;
* Utilização de conexão segura.

### Testes de regressão

Serão executados após correções e atualizações importantes.

O objetivo é verificar se uma alteração realizada no sistema causou falhas em funcionalidades que já estavam funcionando corretamente.

---

## 4. Critérios de Entrada e Saída

### Critérios de Entrada

Os testes poderão ser iniciados quando:

* Os requisitos das funcionalidades estiverem definidos;
* As funcionalidades principais estiverem disponíveis no ambiente de testes;
* O ambiente de testes estiver funcionando;
* Os dados necessários para os testes estiverem disponíveis;
* Os responsáveis pelos testes tiverem acesso ao sistema;
* Os critérios de funcionamento esperados estiverem definidos.

### Critérios de Saída

Os testes serão considerados concluídos quando:

* Todas as funcionalidades principais forem testadas;
* Os cenários de teste prioritários forem executados;
* Não existirem erros críticos ou bloqueadores;
* Os erros de alta prioridade forem corrigidos ou aprovados pela equipe responsável;
* Os testes de regressão forem realizados após as correções;
* O site apresentar funcionamento adequado nos principais navegadores e dispositivos;
* Os resultados dos testes estiverem registrados.

---

## 5. Ambiente de Testes

Os testes serão realizados em um ambiente separado do ambiente de produção.

O ambiente deverá possuir:

* Uma versão atualizada do site;
* Banco de dados de testes, caso seja necessário;
* Dados fictícios para preenchimento dos formulários;
* Computadores e dispositivos móveis;
* Acesso aos principais navegadores;
* Conexão com a internet.

O uso de dados fictícios ajudará a evitar a exposição de informações reais durante os testes.

---

## 6. Recursos e Responsabilidades

Como o projeto possui um time reduzido, as responsabilidades serão divididas da seguinte forma:

### Responsável pelos testes

Será responsável por:

* Criar os cenários e casos de teste;
* Executar os testes;
* Registrar os resultados;
* Identificar e documentar os erros encontrados;
* Acompanhar a correção dos problemas;
* Realizar os testes de regressão.

### Desenvolvedores

Serão responsáveis por:

* Desenvolver as funcionalidades;
* Realizar testes básicos antes de disponibilizar as funcionalidades;
* Corrigir os erros identificados;
* Informar quando as correções estiverem disponíveis para novos testes.

### Responsável pelo projeto ou cliente

Será responsável por:

* Validar se o site atende às necessidades da clínica;
* Avaliar as funcionalidades principais;
* Aprovar a versão final do sistema.

---

## 7. Cronograma Básico

| Etapa | Atividade                                                     | Período                                 |
| ----- | ------------------------------------------------------------- | --------------------------------------- |
| 1     | Análise das funcionalidades e definição dos cenários de teste | Início do projeto                       |
| 2     | Preparação do ambiente e dos dados de teste                   | Início do desenvolvimento               |
| 3     | Execução dos testes funcionais                                | Durante o desenvolvimento               |
| 4     | Execução dos testes de usabilidade e compatibilidade          | Após a conclusão das principais páginas |
| 5     | Registro e correção dos erros encontrados                     | Durante todo o projeto                  |
| 6     | Testes de regressão                                           | Após cada correção importante           |
| 7     | Testes finais e validação                                     | Antes da entrega                        |
| 8     | Aprovação e publicação do site                                | Final do projeto                        |

Os testes serão realizados continuamente durante o desenvolvimento, e não apenas no final do projeto.

---

## 8. Riscos e Contingências

### Risco 1: Falha no formulário de contato ou agendamento

**Possível impacto:** o usuário poderá não conseguir entrar em contato com a clínica ou solicitar uma consulta.

**Contingência:** realizar testes completos dos formulários, validar os campos e verificar o envio das informações.

### Risco 2: Exposição de dados pessoais

**Possível impacto:** informações dos usuários poderão ser acessadas ou utilizadas de forma inadequada.

**Contingência:** utilizar dados fictícios durante os testes, verificar o controle de acesso e realizar testes básicos de segurança.

### Risco 3: Problemas em celulares ou navegadores

**Possível impacto:** o site poderá apresentar erros ou ficar difícil de utilizar em determinados dispositivos.

**Contingência:** realizar testes de compatibilidade nos principais navegadores e em diferentes tamanhos de tela.

### Risco 4: Falta de tempo para executar todos os testes

**Possível impacto:** algumas funcionalidades poderão ser entregues sem a verificação adequada.

**Contingência:** priorizar as funcionalidades mais importantes e os testes com maior risco, como formulários, agendamentos, segurança e navegação.

### Risco 5: Correções causarem novos erros

**Possível impacto:** uma alteração poderá prejudicar funcionalidades que já estavam funcionando.

**Contingência:** executar testes de regressão após cada correção ou atualização importante.

### Risco 6: Indisponibilidade do ambiente de testes

**Possível impacto:** os testes poderão ser interrompidos ou atrasados.

**Contingência:** comunicar o problema à equipe técnica, corrigir o ambiente e reorganizar o cronograma de testes.

---

## 9. Conclusão

O plano de testes foi elaborado considerando as funcionalidades principais do site, o prazo de entrega, a quantidade reduzida de pessoas na equipe e a disponibilidade de um ambiente de testes.

Os testes serão realizados continuamente durante o desenvolvimento, priorizando as funcionalidades que apresentam maior risco e impacto para os usuários.

Com a execução desse plano, será possível identificar falhas, acompanhar as correções e aumentar a qualidade, a segurança e a confiabilidade do site da clínica de psicologia antes da entrega final.
