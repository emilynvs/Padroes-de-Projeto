# 🧩 Composite
- Agrupa objetos de maneira uniforme e utilizando uma hierarquia, como a estrutura de árvore,
  permitindo que objetos individuais/diferentes sejam tratados da mesma forma

---
## 💥 Problema
Um `armário` que pode guardar diversas coisas, como `produtos` ou até mesmo `caixas` e dentro desses `caixas` 
pode possuir mais `produtos`.
Se criar um sistema para esses objetos dentro do armário, poderia causar incompatibilidade tendo em vista que são objetos diferentes

---
## ✅ Solução
O Padrão Composite permite que o seu sistema fique mais flexível, já que em `Java` por exemplo
é necessário saber qual é o objeto a ser tratado.
Utilizar o Composite permite que todos os objetos, caixas vazias, caixas com produtos ou produtos separados possam ser
manipulados de maneira uniforme

---
## Analogia 
- Hierarquia eclesiástica:
  - Papa(nível mais alto, surpervisiona cardeais/bispos)
  - Bispos/Cardeais(podem supervisionar padres)
  - Padres(podem supervisionar diáconos ou fiéis)
  - Diáconos ou leigos(geralmente não supervisionam outros)
  - Component: A interface-> realizarFuncao();
    > interface MembroIgreja {
    void realizarFuncao();
    }
  - Composite 
    - Papa
    - Cardeais/Bispos
    - Padres
  - Leaf(folha)
    - Diáconos
    - Leigos

---
## Vantagens

---
## Desvantagens

---
## Código resumo

    Interface MembroIgreja {
    void realizarFuncao();
    }
    
    class Papa implements MembroIgreja {
    List<MembroIgreja> subordinados = new ArrayList<>();
    
        void realizarFuncao() {
            System.out.println("Papa coordena a Igreja.");
            for (MembroIgreja m : subordinados) {
                m.realizarFuncao();
            }
        }
        void adicionarSubordinado(MembroIgreja m) {
            subordinados.add(m);
        }
    }
    
    class Padre implements MembroIgreja {
    void realizarFuncao() {
    System.out.println("Padre celebra missa.");
    }
    }
    
    class Diacono implements MembroIgreja {
    void realizarFuncao() {
    System.out.println("Diácono auxilia na missa.");
    }
    }

---