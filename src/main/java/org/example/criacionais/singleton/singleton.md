# 🧩 Singleton
- Instancia única
- Fornece um ponto de acesso global a essa instância

---
## 💥 Problema
-  Em determinadas partes do sistema, será necessário trabalhar com a instância única
  - Log de sistemas
  - Gerador de ID
  - etc
- Criar instancias com o método tradicional, ou seja multiplos `new`, geraria mau uso de memória, dados inconsistentes, etc


---
## ✅ Solução
- O padrão Singleton sugere que:
  - Cria-se um construtor padrão privado
  - Cria um método estático de criação que age como um construtor
    - ele verifica se a instância já existe, caso o contrario ele cria uma e envia(retorna)
- Não importa quantas vezes a classe é chamada, vai ser sempre a mesma instância que será retornada
---

## Analogia 
- Identidade(RG, CPF), tendo em vista que cada um possui identidade única

---
## Vantagens

---
## Desvantagens

---
## Código resumo

---