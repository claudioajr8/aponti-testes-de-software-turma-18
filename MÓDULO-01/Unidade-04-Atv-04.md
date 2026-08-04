# Atividade Avaliativa – Testes de Performance

**1. O sistema pode ser considerado aprovado?**

O sistema não pode ser considerado totalmente aprovado, pois apresenta problemas de desempenho durante a execução dos testes. Para que seja aprovado, é necessário que os resultados estejam dentro dos limites definidos nos requisitos de performance, como tempo máximo de resposta, quantidade de usuários suportados e percentual aceitável de erros.

**2. Quais métricas indicam problemas de performance?**

As principais métricas que podem indicar problemas são:

* **Tempo de resposta elevado:** as páginas ou funcionalidades demoram mais do que o esperado para carregar.
* **Alta taxa de erros:** ocorre um aumento de falhas, como erros de servidor ou solicitações que não são concluídas.
* **Baixa quantidade de requisições processadas:** o sistema processa menos operações por segundo do que o esperado.
* **Alto consumo de CPU:** o processador do servidor pode estar trabalhando próximo do limite.
* **Alto consumo de memória:** o uso excessivo de memória pode causar lentidão ou travamentos.
* **Aumento do tempo de resposta com mais usuários:** o sistema perde desempenho à medida que a quantidade de acessos simultâneos aumenta.

**3. Quais possíveis gargalos podem existir?**

Os possíveis gargalos são:

* Banco de dados lento ou com consultas mal otimizadas;
* Servidor com pouca capacidade de processamento;
* Falta de memória disponível;
* Número insuficiente de servidores para atender à demanda;
* Problemas na rede ou baixa largura de banda;
* Código da aplicação pouco otimizado;
* Excesso de acessos simultâneos;
* Falta de mecanismos de cache.

**4. Esse cenário se aproxima mais de Carga, Stress ou Capacidade?**

Esse cenário se aproxima mais de um **Teste de Carga**, pois o objetivo é verificar como o sistema se comporta durante uma quantidade esperada ou elevada de usuários acessando simultaneamente.

Caso a quantidade de usuários ultrapasse o limite previsto e o sistema apresente falhas, travamentos ou indisponibilidade, o cenário também pode apresentar características de um **Teste de Stress**.

**5. O que você recomendaria ao time técnico?**

Recomenda-se que o time técnico:

* Analise os registros de erros e os relatórios de desempenho;
* Otimize as consultas realizadas no banco de dados;
* Verifique o consumo de CPU, memória e rede;
* Melhore e otimize o código da aplicação;
* Utilize mecanismos de cache para reduzir o tempo de resposta;
* Aumente a capacidade dos servidores, caso seja necessário;
* Realize novos testes após as correções;
* Defina limites claros para o tempo de resposta e a quantidade máxima de usuários suportados.

**Conclusão:**

O sistema deve passar por melhorias e novos testes antes de ser considerado totalmente aprovado. As métricas de tempo de resposta, taxa de erros e utilização dos recursos devem ser analisadas para identificar os gargalos e garantir que o sistema funcione de forma estável mesmo com vários usuários acessando ao mesmo tempo.
