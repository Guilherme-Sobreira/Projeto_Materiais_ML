# Projeto Materiais ML
Guilda: Equipe Thunder

![Thunder Logo-export](https://github.com/user-attachments/assets/b5e844e8-ee63-446e-aa99-458ce69dcd8b)

Autores: Guilherme Caetano de Almeida Sobreira, Henrique Valente Nogueira

## Sumário
Esse trabalho pode ser separado em quatro partes principais:

  * __1.__ Intuito do trabalho
    
  * __2.__ Motivações
    
  * __3.__ Resumo do código
    
  * __4.__ Agradecimentos
    
  * __5.__ Referências

## 1. Intuito do trabalho
   O código utiliza inúmeros algoritmos de Aprendizado de máquina para descobrir o índice de refração de um material específico. O índice de refração
   é a medida da fração da velocidade da luz no vácuo com a velocidade da luz em um material, definido por  $$I = \frac{c}{v_2}$$ , onde $$I$$ é o índice de refração,
   $$c$$ é a velocidade da luz no vácuo e $$v_2$$ é a velocidade da luz na substância que a luz atravessa. Para isso, foi usado um dataset [1] contendo diversas informações 
   sobre a estrutura de diversos materiais, como sua estrutura óptica, estrutura cristalina, índice de disperção e quantidade de hidrogênios para treino. Com esses dados,
   ele roda testes com esses algoritmos e gera gráfico comparando o índice de refração previsto e o real.

## 2. Motivações
  O índice de refração é um valor extremamente importante no desenvolvimento de dispositivos ópticos, como lentes, além do estudo de fenômenos físicos, químicos
  e biológicos. No entanto, esse valor ainda é dependente de muitas análises empíricas e testes para descobrir a velocidade que a luz atravessa o material. Ou seja, usar 
  Aprendizado de máquina para poder estimar esse valor sem ter que fazer a análise empírica pode ser a chave para desenvolvimentos tecnológicos no futuro.

## 3. Resumo do código
O Código foi separado nos diversos modelos utilizados. Esses modelos são:
  
  * __1.__ Modelo Baseline:
    
  * __2.__ Modelo linear:
    
  * __3.__ Floresta aleatória:
    
  * __4.__ Modelo K-NN:
    
  * __5.__ Modelo SVM:
  
## Agradecimentos:

Gostaríamos de agradecer ao professor Daniel Roberto Cassar pelas aulas oferecidas durante a disciplina e pelos auxílios com o trabalho

## Referências:

[1] Dataset Origin: https://www.kaggle.com/datasets/vinven7/comprehensive-database-of-minerals?resource=download


