# Classificação dos Cenários de Teste — Manual ou Automatizado

## Objetivo

O objetivo desta atividade é analisar os diferentes cenários de teste do site da clínica de psicologia e definir se cada um deve ser executado de forma manual ou automatizada.

A escolha foi realizada considerando:

* Frequência de execução;
* Necessidade de repetição;
* Estabilidade da funcionalidade;
* Custo e tempo necessários;
* Objetivo do teste;
* Quantidade reduzida de pessoas na equipe.

---

## Cenários de Teste

| Nº | Cenário de Teste                                                               | Abordagem        | Justificativa                                                                                                                                                                              |
| -: | ------------------------------------------------------------------------------ | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|  1 | Verificar se os menus direcionam para as páginas corretas                      | **Automatizado** | É um teste repetitivo e estável. Pode ser executado várias vezes após alterações no sistema, reduzindo o tempo necessário para testes de regressão.                                        |
|  2 | Verificar o funcionamento dos botões e links                                   | **Automatizado** | Os botões e links possuem comportamentos previsíveis e podem ser testados repetidamente. A automação ajuda a identificar rapidamente links quebrados.                                      |
|  3 | Validar os campos obrigatórios do formulário de contato                        | **Automatizado** | A validação dos campos segue regras definidas e pode ser repetida diversas vezes com diferentes dados de teste.                                                                            |
|  4 | Verificar o envio correto do formulário de contato                             | **Automatizado** | É uma funcionalidade importante e deve ser testada sempre que houver alterações. A automação permite executar esse teste com rapidez.                                                      |
|  5 | Testar o login com dados válidos e inválidos                                   | **Automatizado** | O login possui resultados esperados e regras estáveis. Por ser uma funcionalidade importante, deve fazer parte dos testes automatizados de regressão.                                      |
|  6 | Verificar o funcionamento do agendamento de consultas                          | **Automatizado** | O processo possui etapas definidas e pode ser repetido com frequência. A automação ajuda a garantir que o agendamento continue funcionando após atualizações.                              |
|  7 | Avaliar se a navegação pelo site é simples e intuitiva                         | **Manual**       | A facilidade de navegação depende da percepção e da experiência do usuário. Esse tipo de avaliação exige análise humana.                                                                   |
|  8 | Avaliar a clareza dos textos, botões e mensagens                               | **Manual**       | A compreensão das informações é subjetiva e pode variar de acordo com o usuário. Por isso, a avaliação manual é mais adequada.                                                             |
|  9 | Verificar se o layout está organizado e visualmente adequado                   | **Manual**       | A análise da aparência e da organização visual exige avaliação humana e não pode ser totalmente substituída por testes automatizados.                                                      |
| 10 | Verificar se o site se adapta corretamente a celulares, tablets e computadores | **Manual**       | A visualização em diferentes tamanhos de tela deve ser analisada visualmente. Embora parte possa ser automatizada, a verificação manual é importante para identificar problemas de layout. |
| 11 | Verificar o funcionamento do site nos principais navegadores                   | **Automatizado** | Os mesmos cenários podem ser executados repetidamente em diferentes navegadores. A automação reduz o tempo e aumenta a cobertura dos testes.                                               |
| 12 | Verificar se as mensagens de erro são claras e compreensíveis                  | **Manual**       | É necessário avaliar se as mensagens ajudam o usuário a entender o problema e a corrigir a informação.                                                                                     |
| 13 | Verificar se as funcionalidades continuam funcionando após uma atualização     | **Automatizado** | Trata-se de um teste de regressão, que precisa ser executado várias vezes. A automação reduz o esforço e acelera a identificação de falhas.                                                |
| 14 | Avaliar a experiência completa do usuário ao realizar um agendamento           | **Manual**       | O teste deve analisar a facilidade, a clareza e a experiência durante todo o processo, fatores que dependem da avaliação humana.                                                           |
| 15 | Verificar o tempo de carregamento das páginas principais                       | **Automatizado** | O tempo de resposta pode ser medido por ferramentas e comparado com valores definidos, permitindo a repetição dos testes.                                                                  |

---

## Conclusão

A automação será priorizada nos testes que possuem etapas repetitivas, resultados previsíveis e funcionalidades estáveis, como validação de formulários, login, menus, links, agendamento e testes de regressão.

Os testes manuais serão utilizados principalmente para avaliar a experiência do usuário, a facilidade de navegação, a clareza das informações e a aparência do site.

A combinação das duas abordagens é a mais adequada para o projeto. Os testes automatizados ajudam a economizar tempo e reduzir o esforço da equipe, enquanto os testes manuais permitem avaliar aspectos subjetivos que dependem da percepção humana.
