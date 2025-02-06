# Trabalho Final Programação Matemática

Alunos:

Vítor Pires Zini - 202110169
Luiz Filipe Bartelega Penha - 202111082

# Contextualização

Fake news são informações falsas ou enganosas divulgadas como verdadeiras, geralmente em redes sociais. Com títulos sensacionalistas, buscam engajar emocionalmente e incentivar o compartilhamento sem verificação.

Seus impactos incluem a manipulação da opinião pública, desinformação em crises, danos à reputação e riscos à saúde, como visto na pandemia de COVID-19.

O combate exige educação midiática, ferramentas tecnológicas e esforços colaborativos para limitar sua disseminação.

# Enunciado do Problema

O problema descrito no enunciado trata da disseminação de notícias falsas (fake news) em uma rede de computadores modelada por um grafo direcionado G=(V,E), onde:

Vértices (V): Representam os servidores que processam as informações.

Arcos (E): Representam os enlaces de comunicação entre os servidores.

O objetivo é reduzir o número de servidores que uma notícia falsa pode alcançar em um período de tempo T. Para isso, o Setor de Tecnologia da Informação (STI) do governo federal possui α recursos tecnológicos (como softwares auxiliares) que podem ser aplicados aos servidores para retardar a propagação da notícia falsa.

Cada recurso i (onde i=1,…,α) fica disponível no instante βi e, quando aplicado a um servidor u, aumenta o tempo de transmissão da notícia falsa no enlace (u,v) de tuv para tuv+δ, onde δ>0 é um atraso de propagação.

A solução do problema consiste em determinar a alocação desses recursos aos servidores, com as seguintes restrições:

Cada servidor pode receber no máximo um recurso.

Um recurso i é alocado no menor tempo βi.

O objetivo final é minimizar a quantidade de servidores que a notícia falsa pode alcançar em um tempo menor ou igual a T.

# Instruções de Uso do Algoritmo de Busca Local Iterada (ILS) para Fake News

Este documento fornece as instruções necessárias para executar o algoritmo de Busca Local Iterada (ILS) aplicado à minimização da disseminação de fake news. Siga os passos abaixo para configurar e executar o programa.

## Entradas Necessárias

Ao iniciar o programa, serão solicitadas as seguintes entradas:

1. **Nome do Arquivo de Resultado Final**  
   - **Prompt:**  
     ```
     Digite o nome do arquivo que será gravado o resultado final do algoritmo:
     ```  
   - **Descrição:** Informe o nome do arquivo (por exemplo, `resultado.txt`) onde o algoritmo salvará o resultado final, que corresponde ao número de servidores afetados pela fake news conforme a melhor solução encontrada.

2. **Quantidade Máxima de Iterações**  
   - **Prompt:**  
     ```
     Digite o quantidade máxima de iterações:
     ```  
   - **Descrição:** Especifique o número máximo de iterações que o algoritmo deverá executar. Este parâmetro determina a profundidade da busca local e, consequentemente, o tempo de execução.

3. **Quantidade de Perturbações**  
   - **Prompt:**  
     ```
     Digite a quantidade de perturbações:
     ```  
   - **Descrição:** Indique quantas perturbações (trocas intensas) serão realizadas quando a busca local não conseguir melhorar a solução. Este valor auxilia o algoritmo a escapar de ótimos locais e explorar novas regiões do espaço de soluções.

4. **Nome do Arquivo de Instância**
   - **Prompt:**  
     ```
     Digite o nome do arquivo de instância:
     ```  
   - **Descrição:** Forneça o nome do arquivo que contém os dados da instância do problema.

# Estrutura do Repositório

- Colab Notebook contendo o código fonte que contém a Metaheurística que resolve o problema
- Relatório contendo:
    - Introdução
    - Formulação (Modelagem de Programação Inteira + Formulação da Metaheurística)
    - Descrição da solução (Como o problema foi resolvido)
    - Resultados e Discussão (Apresentação das soluções encontradas e suas análises)
    - Conclusão (Descrição geral do problema e solução)
    - Bibliografia (Materiais utilizados para auxiliar o desenvolvimento do trabalho)
