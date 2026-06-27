<script type="text/x-mathjax-config">
  MathJax.Hub.Config({
    tex2jax: {
      inlineMath: [['$','$'], ['\\(','\\)']],
      displayMath: [['$$','$$'], ['\\[','\\]']],
      processEscapes: true
    }
  });
</script>

<script type="text/javascript" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# Plano de Trabalho

1. Montar o relatório apresentando as inconsistências experimentais identificadas:

- Na geração de instâncias, de rotas conflitantes, com set differences entre os meus conjuntos e o do joão;
- Na implementação da restrição de exclusão de operações mutuas em rotas conflitantes (restrições 446_1 e 446_2);

2. Dizer que mesmo sem equivalência comparativa (por conta dos poliedros distintos), a nossa implementação apresentou resultados de FO melhores do que a implementação do João, mesmo com as inconsistências experimentais identificadas.

3. Apresentar inconsistências no balanceamento de estoques (baseado no balanceamento futuro) que deixa o estoque do período 1 desvinculado ao estoque inicial.

4. Apresentar inconsistências da restrição de limitação do escoamento, a $\sum_{r \in R_y[s]} (c^{r}_{y}[r]\ y_r[r, p, t]) \leq e[s, p, t] \, \forall s \in S, p \in P, t \in T$, que não limita o escoamento y ao estoque do período anterior, mas sim, ao do periodo corrente que é modificado pela entrada de minérios por $r_x[s]$

5. Apresentar o argumento da impossibilidade comparativa entre as implementações, devido às inconsistências experimentais identificadas que indelevelmente modificam o poliedro do espaço de soluções entre uma implementação e outra, o que pode acarretar nas diferenças de resultados identificadas.

6. Ainda assim, apresentar os resultados de 5 implementações fáceis realizadas.

7. Agora, o que explica essas melhorias? Porque ao reproduzir o experimento do João com a retirada da inconsistência experimental, ainda assim nossa solução apresentou resultados melhores. Portanto, o poliedro está diferente, mas como caracterizar essas diferenças? Isso já entra no âmbito especulativo, é muito difícil, porque é associado à necessidade de provar um fato negativo, como, por exemplo, outra inconsistência de restrições ou de modelo do trabalho do João, que não conseguimos identificar de imediato. Entretanto, a verificação do nosso modelo é mais assertiva, pois, a equivalência matemática em conformidade às notações da dissertação é imediata, o JuMP impõe a notação algébrica, basicamente a mesma da formulação matemática.

- Isso vêm na esteira de que os indicios sugerem que essa diferença de resultados pode ser explicada por outras inconsistências experimentais ainda não identificadas, mas, que podem ser sementes de trabalhos futuros.

8. Com isso concluimos que nossos resultados estão consistentes, que obtivemos melhorias e avançamos o estado da arte interno das pesquisas feitas pelo grupo. A identificação de uma inconsistência e sua correção são melhorias significativas.
