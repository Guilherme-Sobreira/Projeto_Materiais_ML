# Projeto Materiais ML
Guilda: Equipe Thunder

![Thunder Logo-export](https://github.com/user-attachments/assets/b5e844e8-ee63-446e-aa99-458ce69dcd8b)

Autores: Guilherme Caetano de Almeida Sobreira, Henrique Valente Nogueira

## Separação de arquivos
 * __Dataset:__ Possui o Dataset [1] utilizado no código do trabalho
 * __Code:__ Contém o código completo do trabalho

## Sumário
Esse trabalho pode ser separado em quatro partes principais:

  * __1.__ Intuito do trabalho
    
  * __2.__ Motivações
    
  * __3.__ Resumo do código
    
  * __4.__ Agradecimentos
    
  * __5.__ Referências

### 1. Intuito do trabalho
   O código utiliza inúmeros algoritmos de Aprendizado de máquina para descobrir o índice de refração de um material específico. O índice de refração
   é a medida da fração da velocidade da luz no vácuo com a velocidade da luz em um material, definido por  $$I = \frac{c}{v_2}$$ , onde $$I$$ é o índice de refração,
   $$c$$ é a velocidade da luz no vácuo e $$v_2$$ é a velocidade da luz na substância que a luz atravessa. Para isso, foi usado um dataset [1] contendo diversas informações 
   sobre a estrutura de diversos materiais, como sua estrutura óptica, estrutura cristalina, índice de disperção e quantidade de hidrogênios para treino. Com esses dados,
   ele roda testes com esses algoritmos e gera gráfico comparando o índice de refração previsto e o real.

### 2. Motivações
  O índice de refração é um valor extremamente importante no desenvolvimento de dispositivos ópticos, como lentes, além do estudo de fenômenos físicos, químicos
  e biológicos. No entanto, esse valor ainda é dependente de muitas análises empíricas e testes para descobrir a velocidade que a luz atravessa o material. Ou seja, usar 
  Aprendizado de máquina para poder estimar esse valor sem ter que fazer a análise empírica pode ser a chave para desenvolvimentos tecnológicos no futuro.

### 3. Resumo do código
O dataframe foi extraído de uma base didática de dados a respeito de mineralogia. Cada coluna está relacionada a dados físicos ou químicos dos minerais, e suas informações podem ser consultadas na referência [1].
O Código foi separado nos diversos modelos utilizados e pode ser acessado na pasta 'Código'. Nele, diferentes modelos serão testados para analisar a eficiência em prever os índices de refração. Esses modelos são:
  
  * __1. Modelo Baseline:__ Usa o modelo de linha de base para gerar previsões baseado nos valores.
    
  * __2. Modelo linear:__ Utilisa regresão linear para gerar previsões baseado nos valores.

  * __3. Árvore de decisão:__ Usa o algoritmo de árvore de decisão para calcular os valores.
  
  * __4. Floresta aleatória:__ Utiliza o algoritmo de floresta aleatória, que é uma versão menos enviesada do Árvore de decisão, para calcular os valores.
    
  * __5. Modelo K-NN:__ Usa o bodelo regressivo de k números vizinhos para calcular os valores.
    
  * __6. Modelo SVM:__ Utiliza Support Vector Machine (Máquina de vetores de suporte) para calcular os valores.
  
### 4. Agradecimentos:

Gostaríamos de agradecer ao professor Daniel Roberto Cassar pelas aulas oferecidas durante a disciplina e pelos auxílios com o trabalho

### 5. Referências:

[1] Dataset Origin: https://www.kaggle.com/datasets/vinven7/comprehensive-database-of-minerals?resource=download
[2] Material didático - ATP - 203 (Aprendizado de Máquina) - Ministrada pelo professor Daniel Cassar.
