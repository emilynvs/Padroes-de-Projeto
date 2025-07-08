# 🧩 Factory Method
- Define uma interface para a criação do objeto, permitindo que as subclasses decidam qual subclasse instanciar
- 

---
## 💥 Problema
- Imagine que sua loja de venda de chinelos possui somente métodos para a venda desse produto,
porém com as mudanças das estações você precisa se adequar para conseguir vender, nas épocas mais frias
seria interessante ter calçados para esse tempo. Porém, toda a sua lógica de negócio do programa
está voltada para a venda de chinelos
  - Uma solução, seria reformular o código para ele poder aceitar venda de calçados para estações frias,
  porém, e se houver outros calçados que os clientes procuram?
    - Teria que reformular o código novamente, o transformando em uma sopa com tudo o que tem direito,
    e chegará um momento em que não será mais possível manter devido à mistura de códigos

---
## ✅ Solução
- O Factory Method, propõe que crie uma ‘interface’ base para as subclasses implementarem e uma fábrica especial para retornar os diferentes produtos
  - Nesse caso, teríamos as classes `chinelos`,`botas`, `tenis` que implementariam a ‘interface’ `calçado` e as classes entrariam em uma fabrica especial
    (nesse exemplo seria a `loja`) que iria instanciar os calçados `chinelos`,`botas`, `tenis` de maneira mais simplificada
  - Desse modo, há a possibilidade de adicionar novas classes de calçados sem muita dificuldade 

---

## Analogia 
- Lojas de varejos e supermercados, independente do que o cliente comprar sempre será um produto(a interface base seria produto)
  - Além disso, os supermercados não precisam dos detalhes de como o produto é fabricado, ele só precisa 
  chamar o fornecedor para entregar o que o mercado precisa

---
## Vantagens

---
## Desvantagens

---
## Código resumo

---