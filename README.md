# provaDidatica173

Material para a Prova Didática do Concurso Docente para professor Adjunto do Centro de Tecnologia da UFSM, Departamento de Eletrônica e Computação, realizado no dia 11/05/2023.

## Instruções

### Gerando os slides

Para gerar os slides da aula, siga o seguinte passo-a-passo:

1. Abrir um console do Python na pasta do projeto
2. Digitar o seguinte comando no console:

   ```bash
   jupyter nbconvert --to slides slides.ipynb
   ``` 

3. Caso você queira gerar os slides e vê-los imediatamente, digite o seguinte comando:
   
   ```bash
   jupyter nbconvert --to slides slides.ipynb --post serve
   ``` 