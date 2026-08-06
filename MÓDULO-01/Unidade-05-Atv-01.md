# Estratégia de Testes — Site de uma Clínica de Psicologia

## 1. Objetivo da Estratégia

O objetivo desta estratégia de testes é garantir que o site da clínica de psicologia funcione corretamente, seja seguro, fácil de utilizar e ofereça uma experiência confiável aos usuários.

Como o sistema será utilizado por pessoas reais e poderá conter informações pessoais e sensíveis, os testes deverão priorizar a proteção dos dados, o funcionamento das funcionalidades principais e a facilidade de uso.

A estratégia também busca identificar e corrigir problemas durante o desenvolvimento, reduzindo a possibilidade de falhas após a publicação do site.

### O que é mais importante garantir com os testes?

Os principais pontos que devem ser garantidos são:

* O funcionamento correto das funcionalidades principais do site;
* A segurança e a privacidade dos dados dos usuários;
* O funcionamento adequado dos formulários de contato e agendamento;
* A facilidade de navegação e utilização;
* A compatibilidade com diferentes dispositivos e navegadores;
* A estabilidade do sistema após atualizações e correções.

### Aspectos que merecem maior atenção

Os aspectos que receberão maior atenção são:

* Cadastro e envio de informações pelos usuários;
* Formulários de contato;
* Agendamento de consultas, caso essa funcionalidade esteja disponível;
* Proteção dos dados pessoais;
* Login e acesso a áreas restritas, caso existam;
* Navegação entre as páginas;
* Exibição correta do conteúdo em celulares e computadores;
* Mensagens de erro e validação dos campos.

Esses pontos são prioritários porque falhas nessas áreas podem prejudicar a experiência do usuário, causar perda de informações ou comprometer a privacidade dos dados.

---

## 2. Tipos de Testes Prioritários

### Testes funcionais

Os testes funcionais terão alta prioridade. Eles serão utilizados para verificar se as funcionalidades do site estão funcionando conforme os requisitos definidos.

Serão testados, por exemplo:

* Navegação entre as páginas;
* Botões e links;
* Formulários de contato;
* Campos obrigatórios;
* Validação de informações;
* Envio de mensagens;
* Agendamento de consultas;
* Login e acesso a áreas restritas, caso existam.

Esses testes são importantes porque o site possui diversas funcionalidades e será utilizado por usuários reais.

### Testes de usabilidade

Os testes de usabilidade também terão alta prioridade. Eles verificarão se o site é simples, organizado e fácil de utilizar.

Serão avaliados:

* Facilidade para encontrar informações;
* Clareza dos textos e botões;
* Organização das páginas;
* Facilidade para preencher formulários;
* Compreensão das mensagens de erro;
* Facilidade para realizar um agendamento ou entrar em contato.

Esses testes são importantes porque os usuários devem conseguir utilizar o site sem dificuldades.

### Testes de segurança

Os testes de segurança terão alta prioridade devido à possibilidade de o sistema armazenar ou receber dados pessoais e informações sensíveis.

Serão verificados:

* Proteção dos dados enviados pelos usuários;
* Controle de acesso às áreas restritas;
* Segurança do login, caso exista;
* Validação dos dados informados nos formulários;
* Proteção contra acessos não autorizados;
* Uso adequado de conexões seguras.

### Testes de compatibilidade

Os testes de compatibilidade terão prioridade média a alta.

O site será testado em:

* Computadores;
* Celulares;
* Tablets;
* Diferentes navegadores, como Google Chrome, Microsoft Edge e Mozilla Firefox.

Esses testes são importantes porque os usuários poderão acessar o site por diferentes dispositivos.

### Testes de regressão

Os testes de regressão serão realizados sempre que houver uma correção ou inclusão de uma nova funcionalidade.

O objetivo é verificar se uma alteração realizada no sistema não causou problemas em funcionalidades que já estavam funcionando corretamente.

### Testes com menor prioridade

Os testes de carga, estresse e capacidade terão menor prioridade no início do projeto.

A justificativa é que o site será desenvolvido por uma equipe reduzida e possui um prazo definido. Dessa forma, os esforços iniciais serão concentrados nas funcionalidades principais, na segurança e na usabilidade.

Entretanto, testes básicos de desempenho poderão ser realizados antes da entrega para verificar se as páginas apresentam um tempo de resposta adequado.

---

## 3. Abordagens de Teste

### Testes realizados manualmente

Os testes manuais serão utilizados principalmente para verificar:

* Navegação pelo site;
* Facilidade de uso;
* Organização das páginas;
* Clareza dos textos;
* Funcionamento dos formulários;
* Comportamento dos botões e links;
* Aparência do site em diferentes dispositivos;
* Mensagens apresentadas ao usuário;
* Experiência durante o agendamento ou contato.

Os testes manuais são importantes porque permitem analisar a experiência do usuário e identificar problemas que podem não ser percebidos por testes automatizados.

### Testes que poderão ser automatizados

Os testes automatizados poderão ser utilizados para:

* Validar o funcionamento de páginas importantes;
* Testar formulários;
* Verificar campos obrigatórios;
* Testar o login, caso exista;
* Verificar funcionalidades repetitivas;
* Executar testes de regressão;
* Confirmar que os principais links e botões continuam funcionando.

A automação será aplicada principalmente aos testes repetitivos e às funcionalidades mais importantes do sistema.

### Justificativa da combinação

A combinação de testes manuais e automatizados foi escolhida porque o projeto possui um time reduzido e está em desenvolvimento ativo.

Os testes manuais serão importantes para avaliar a experiência do usuário, enquanto os testes automatizados ajudarão a economizar tempo e permitirão repetir verificações importantes após cada atualização.

Dessa forma, será possível utilizar os recursos disponíveis de maneira mais eficiente.

---

## 4. Riscos e Mitigação

### Principais riscos do sistema

Os principais riscos identificados são:

1. **Falha nos formulários de contato ou agendamento**

O usuário pode não conseguir enviar uma mensagem ou solicitar uma consulta.

**Mitigação:** realizar testes funcionais, validar os campos e testar o envio das informações.

2. **Exposição ou perda de dados pessoais**

Informações enviadas pelos usuários podem ser acessadas ou utilizadas de forma inadequada.

**Mitigação:** realizar testes de segurança, validar o controle de acesso e verificar a proteção dos dados.

3. **Dificuldade de utilização**

Os usuários podem ter dificuldades para encontrar informações ou utilizar as funcionalidades.

**Mitigação:** realizar testes de usabilidade e avaliar a organização, os textos e a navegação.

4. **Problemas em dispositivos ou navegadores diferentes**

O site pode funcionar corretamente em um navegador, mas apresentar erros em outros.

**Mitigação:** realizar testes de compatibilidade em diferentes navegadores, computadores e dispositivos móveis.

5. **Novas alterações causarem erros em funcionalidades existentes**

Uma correção ou nova funcionalidade pode gerar falhas em partes que já estavam funcionando.

**Mitigação:** executar testes de regressão após cada alteração importante.

6. **Atrasos no cronograma**

Problemas identificados apenas no final do desenvolvimento podem atrasar a entrega.

**Mitigação:** realizar testes continuamente durante o projeto, permitindo que os erros sejam encontrados e corrigidos mais cedo.

---

## 5. Recursos e Cronograma

### Pessoas envolvidas

Como o projeto possui uma equipe reduzida, os testes poderão ser realizados por:

* 1 responsável pela qualidade e pelos testes;
* Desenvolvedores realizando testes técnicos e verificações das funcionalidades desenvolvidas;
* Participação do responsável pelo projeto na validação final.

O responsável pelos testes será encarregado de planejar os cenários, executar os testes, registrar os problemas encontrados e acompanhar as correções.

### Momentos em que os testes ocorrerão

Os testes serão realizados durante todo o desenvolvimento do projeto.

As principais etapas serão:

* **Início do projeto:** análise dos requisitos e identificação dos riscos;
* **Durante o desenvolvimento:** testes das funcionalidades à medida que forem implementadas;
* **Após cada correção ou atualização:** execução de testes de regressão;
* **Antes da entrega:** execução de testes completos das funcionalidades principais, segurança, usabilidade e compatibilidade;
* **Após a publicação:** acompanhamento do funcionamento do sistema e correção de possíveis problemas.

### Os testes serão contínuos ou concentrados?

Os testes serão realizados de forma contínua.

Essa decisão foi tomada porque o sistema está em desenvolvimento ativo e sofrerá evoluções e correções ao longo do projeto.

A realização contínua dos testes permite identificar problemas mais cedo, reduzir o custo das correções e diminuir o risco de encontrar muitos erros apenas próximo da data de entrega.

---

## 6. Conclusão

A estratégia proposta prioriza as funcionalidades mais importantes, a segurança dos dados, a facilidade de uso e a estabilidade do site.

A utilização combinada de testes manuais e automatizados permitirá aproveitar melhor os recursos do time reduzido. Os testes serão realizados continuamente durante o desenvolvimento, com maior atenção às funcionalidades que apresentam riscos mais elevados.

Essa estratégia busca garantir que o site da clínica de psicologia seja confiável, seguro, acessível e adequado às necessidades dos usuários, mesmo considerando as limitações de prazo e de equipe do projeto.
