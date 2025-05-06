# **Validação de Dados com Great Expectations**

## **Descrição do Projeto**

Este projeto utiliza o framework **Great Expectations** para realizar validações de dados em um conjunto de dados relacionados ao sono. O objetivo é garantir que os dados de entrada atendam a critérios pré-estabelecidos, como valores ausentes, intervalos válidos, e conformidade com as expectativas definidas. <br><br>O Great Expectations é uma ferramenta para realizar testes de qualidade de dados, proporcionando uma forma estruturada e automatizada de validar, documentar e acompanhar a integridade dos dados ao longo do tempo.

## **O que é o Great Expectations?**

O **Great Expectations (GE)** é uma ferramenta open-source para validação, documentação e perfil de dados. Ele permite que os analistas de dados e cientistas de dados definam expectativas claras sobre a qualidade e integridade dos dados em seus pipelines. Essas expectativas podem ser validadas automaticamente, e o GE pode gerar relatórios documentados sobre os resultados dessas validações.

Com o GE, é possível verificar, por exemplo:
- Se os dados seguem um formato esperado.
- Se os valores estão dentro de intervalos válidos.
- Se as colunas não contêm valores nulos.
- Se os dados são consistentes e atendem a outras regras de negócios.

Além disso, o GE permite gerar documentação dos dados e dos testes, o que facilita a rastreabilidade e transparência ao longo do ciclo de vida dos dados.

## **Funcionalidades Implementadas**

Neste projeto, utilizamos o Great Expectations para validar os dados em um conjunto relacionado a métricas de sono. As validações implementadas incluem:

1. **Verificação de Valores Ausentes:**
   - Garantir que as colunas de dados não contenham valores nulos (como "Sleep efficiency", "Age", "Sleep duration").
   
2. **Validação de Intervalos Válidos:**
   - As colunas como "Age", "Sleep efficiency" e "Sleep duration" devem estar dentro de intervalos específicos, definidos como:
     - **Age**: Entre 18 e 100 anos.
     - **Sleep efficiency**: Entre 0.0 e 1.0.
     - **Sleep duration**: Entre 3 e 12 horas.
   
3. **Verificação de Conjunto de Valores Esperados:**
   - A coluna "Gender" deve ter apenas valores válidos, que são "Male" ou "Female".
   
4. **Verificação de Somatório de Percentuais:**
   - A soma das porcentagens de sono (REM, Deep, Light) deve ser aproximadamente igual a 100%.
   
5. **Geração de Relatórios:**
   - O GE gera um relatório HTML com o resultado das validações, mostrando quais expectativas foram atendidas ou falharam. Este relatório pode ser salvo localmente e aberto no navegador.

## **Conclusão**
Este projeto utiliza Great Expectations para validar um conjunto de dados relacionados ao sono, aplicando expectativas rigorosas para garantir a qualidade dos dados. O uso do GE oferece uma abordagem robusta para validar dados, documentar o processo e garantir a confiança nos dados que são utilizados em análises e relatórios.

## **Dataset utilizado:**
https://www.kaggle.com/code/thainazanfolin/estilo-de-vida-e-efici-ncia-do-sono
