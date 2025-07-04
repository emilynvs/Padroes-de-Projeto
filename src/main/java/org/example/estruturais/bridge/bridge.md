# 🧩 Bridge
- Tem a intenção de desacoplar uma abstração da sua implementação
para que ambas possam evoluir independentemente
- Será a ponte para ambas as partes poderem interagir

---
## 💥 Problema
Imagine que você possui um sistema de fábrica com três classes(setores), a cada classe criada é necessário
criar cinco classes de funcionários(`Gerente`, `Almoxarife`, `Supervisor`,`Operador de Máquina`, `Programador da Produção`). 
Desse modo, para realizar alguma manutenção, será necessário fazer manutenção em toda a aplicação 

---
## ✅ Solução
Para evitar a criação de múltiplas classes é necessário separar a classe de funcionários com as classes de setores.
Criando uma classe que servirá como `ponte` entre funcionários e setores

---
## Analogia 
- A maneira como podemos acessar a fonte do conteudo e juntar como a forma que estuda
  - Forma de estudar(Abstração):Ler, assistir, ouvir audio
  - Fonte de conteúdo(Implementação): PDF, Youtube, Livro físico, etc
- Isso evita criar classes para todas as combinações possíveis, como:
  - LerPDF 
  - LerLivroFísico 
  - AssistirYouTube 
  - OuvirAudiobook, etc
- Resumindo, o padrão Bridge funciona como uma “ponte” que une a forma de estudar com a fonte de conteúdo,
possibilitando combinações como:
  - Estudar por leitura + PDF
  - Estudar por leitura + Livro físico

---
## Vantagens

---
## Desvantagens

---
## Código resumo

---