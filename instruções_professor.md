# Instruções (para o professor)

## Gerando os slides

Para gerar os slides da aula, siga o seguinte passo-a-passo:

1. Abra um console do Python na pasta do projeto
2. Digite o seguinte comando no console:

   ```bash
   jupyter nbconvert --to slides slides.ipynb
   ``` 

3. Caso você queira gerar os slides e vê-los imediatamente, digite o seguinte comando:
   
   ```bash
   jupyter nbconvert --to slides slides.ipynb --post serve
   ``` 