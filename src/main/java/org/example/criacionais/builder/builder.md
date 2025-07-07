# 🧩 Builder
- Permite a construção do objeto passo a passo, possibilitando produzir
diferentes tipos e representações do objeto com o mesmo código usado para construi-lo

---
## 💥 Problema
- O código para a construção do objeto precisa de uma inicialização passo a passo, 
possuindo múltiplos parâmetros para ser instanciado
- Mas e se cada objeto tiver algum parâmetro "único"? E se o construtor padrão não for o suficiente?
  - Pode-se criar subclasses, porém chegará em um momento que vai ser difícil de manter o código
  - Pode juntar todos os paramentos em um único construtor, o transformando em um monstro, e usar `null` para os que não forem necessários para o objeto cliente, 
porém também ficará extenso e a maioria dos parâmetros acaba não sendo utilizada pelo cliente

---
## ✅ Solução
- Com o builder, realiza-se a extração do construtor padrão para fora da sua classe original
- Esse padrão concede a possibilidade de criar novas classes para a construção 
de um objeto, com isso um mesmo objeto pode ser criado de maneiras diferentes
- É útil quando você precisa criar várias representações de um produto

---

## Analogia 
- Um ator pode receber os parametros: 
  - figurino, 
  - maquiagem, 
  - personalidade 
- Com base nesses parâmetros é possível criar inúmeros tipos de personagem 
usando o mesmo molde(ator)
- O ator é o construtor (builder) que, passo a passo transforma os parâmetros recebidos em uma
representação final: o personagem

---
## Vantagens

---
## Desvantagens

---
## Código resumo

---