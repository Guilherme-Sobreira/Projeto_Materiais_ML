# Projeto Materiais ML
Guilda: Equipe Thunder

![Thunder Logo-export](https://github.com/user-attachments/assets/b5e844e8-ee63-446e-aa99-458ce69dcd8b)

Autores: Guilherme Caetano de Almeida Sobreira, Henrique Valente Nogueira

## Separação de arquivos
 * __Dataset:__ Possui o Dataset [1] utilizado no código do trabalho
 * __Código:__ Contém o código completo do trabalho

## Sumário
Esse trabalho pode ser separado em quatro partes principais:

  * __1.__ Intuito do trabalho
    
  * __2.__ Motivações
    
  * __3.__ Resumo do notebook
    
  * __4.__ Agradecimentos
    
  * __5.__ Referências

### 1. Intuito do trabalho
   O código utiliza inúmeros algoritmos de Aprendizado de máquina para descobrir o índice de refração de um material específico. O índice de refração
   é a medida da fração da velocidade da luz no vácuo com a velocidade da luz em um material, definido por  $$I = \frac{c}{v_2}$$ , onde $$I$$ é o índice de refração,
   $$c$$ é a velocidade da luz no vácuo e $$v_2$$ é a velocidade da luz na substância que a luz atravessa. Para isso, foi usado um dataset [1] contendo diversas informações 
   sobre a estrutura de diversos materiais, como sua estrutura óptica, estrutura cristalina, índice de dispersão e quantidade de hidrogênios para treino. Com esses dados,
   ele roda testes com esses algoritmos e gera gráfico comparando o índice de refração previsto e o real.

### 2. Motivações
  O índice de refração é um valor extremamente importante no desenvolvimento de dispositivos ópticos, como lentes, além do estudo de fenômenos físicos, químicos
  e biológicos. No entanto, esse valor ainda é dependente de muitas análises empíricas e testes para descobrir a velocidade que a luz atravessa o material. Ou seja, usar 
  Aprendizado de máquina para poder estimar esse valor sem ter que fazer a análise empírica pode ser a chave para desenvolvimentos tecnológicos no futuro.

### 3. Resumo do notebook
O notebook contém a 
O dataframe foi extraído de uma base didática de dados a respeito de mineralogia. Cada coluna está relacionada a dados físicos ou químicos dos minerais, e suas informações podem ser consultadas em detalhes na referência [1]. Como um leve resumo, o DataFrame é separado em:

 * __1. `index`:__ Valor de index para cada mineral
 * __2. `column`:__ Coluna para cada classificassão do material. As colunas estão separadas em:
   * __2.1. Nome:__ Nome do material
   * __2.2. Crystal Structure:__ Indica a estrutura que as moléculas estâo arranjadas no espaço
   * __2.3. Mohs Hardness:__ Escala de dureza dos minerais, ou seja, o quanto esses materiais são resistentes à riscagem.
   * __2.4. Diaphaneity:__ Indica a capacidade da luz passar pelo mineral, sendo uma escala de dados categóricos e ordinais de transparência já traduzida para dados numéricos. 
   * __2.5. Specific Gravity:__ Valor da razão entre a densidade do mineral e a densidade da água.
   * __2.6. Optical:__ Define como as propiedades ópticas mudam de acordo com a direcão observada. Podem ser isotrópicas, biaxiais ou anisotrópicas.
   * __2.7. Refractive Index:__ Valor da razão entre a velocidade da luz no material e a velocidade da luz no vácuo.
   * __2.8. Dispersion:__ Indica a mudança do índice de refração de um material em função da frequência da luz aplicada.
   * __2.9. Elementos:__ Mostra a quantidade de átomos/grupos funcionais de um elemento na fórmula do mineral. Há uma coluna para cada elemento da tabela periódica e para alguns grupos funcionais.
   * __2.10. Count:__ Quantidade de átomos na fórmula do mineral.
   * __2.11. Molar Mass:__ Valor da massa molar de cada material.
   * __2.12. Molar Volume:__ Valor do volume molar de cada material.
   * __2.13. Calculated Density:__ Valor da razão entre a massa molar e o volume em massa.

O Código foi separado nos diversos modelos utilizados e pode ser acessado na pasta 'Código'.
Primeiramente, foi feito uma sequência de diversos tratamento de dados, para gerar valores melhores e com menos ruído para trabalhar.
Após isso, diferentes modelos serão testados para analisar a eficiência em prever os índices de refração. Esses modelos são:
  
  * __1. Modelo Baseline:__ Usa o modelo de linha de base para gerar previsões baseado nos valores.
    
  * __2. Modelo linear:__ Utiliza regressão linear para gerar previsões baseado nos valores.

  * __3. Árvore de decisão:__ Usa o algoritmo de árvore de decisão para calcular os valores.
  
  * __4. Floresta aleatória:__ Utiliza o algoritmo de floresta aleatória, para calcular os valores.
    
  * __5. Modelo K-NN:__ Usa o modelo regressivo de k-números vizinhos para calcular os valores.
    
  * __6. Modelo SVM:__ Utiliza Support Vector Machine (Máquina de vetores de suporte) para calcular os valores.

Por último, foi adicionado modelos de hiperparâmetros melhorar alguns algoritmos específicos. Mais especificamente, há a aplicação no algoritmo de SVM e no algoritmo de Floresta aleatória.
  
### 4. Agradecimentos:

Gostaríamos de agradecer ao professor Daniel Roberto Cassar pelas aulas oferecidas durante a disciplina e pelos auxílios com o trabalho

### 5. Referências:

[1] Dataset Origin: https://www.kaggle.com/datasets/vinven7/comprehensive-database-of-minerals?resource=download

[2] Material didático - ATP - 203 (Aprendizado de Máquina) - Ministrada pelo professor Daniel Cassar.
