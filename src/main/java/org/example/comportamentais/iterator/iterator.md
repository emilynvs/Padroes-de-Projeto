# 🧩 Iterator
- Possibilita acessar os elementos de um objeto sequencialmente

---
## 💥 Problema
- Imagine que você tem uma empresa de rotas, com trajetos que possuem pontos intermediários (paradas, entregas, o que você imaginar)
- Porém, está focado para a sua cidade, com o tempo seu negócio toma uma proporção maior, abrangendo todo o país
- As estruturas internas para armazenar rotas variam — algumas podem ser listas, outros mapas, outros bancos de dados. 
- Você precisa fornecer ao usuário uma maneira simples de percorrer a rota passo a passo, sem que ele precise saber como a rota está implementada internamente.
---
## ✅ Solução
- A solução é poder acessar cada rota sequencialmente, independente do ponto inicial e final do usuário, sem expor a estrutura interna.
- Permitindo trocar o formato de armazenamento sem afetar o código

---

## Analogia
- Chamada, o professor passa aluno por aluno
- Lista de reprodução do spotify