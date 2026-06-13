# Modelando o Iphone com UML - Desafio de Projeto [DIO](www.dio.me)

## POO - Desafio
## Resolução
Criei um diagrama no mermaid onde adicionei todas as funções, um diagrama facil de ler e entender cada parte.

## Autor
- [Luiz Almeida](https://github.com/LuizAlmeidaF)


## Diagrama UML (Mermaid)

```mermaid
classDiagram
    class ReproductorMusical {
        -musicaAtual: String
        -estaReproduzindo: boolean
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }
    
    class AparelhoTelefonico {
        -numeroAtual: String
        -emChamada: boolean
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }
    
    class NavegadorInternet {
        -urlAtual: String
        -abas: List
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    
    class iPhone {
        -modelo: String
        -armazenamento: int
    }
    
    iPhone *-- ReproductorMusical
    iPhone *-- AparelhoTelefonico
    iPhone *-- NavegadorInternet
```
