# PROFESSOR DE INFORMÁTICA - IFPI 2026

## CONHECIMENTOS ESPECÍFICOS

Início: 11/02/2026

Algoritmos Lógica de Programação e Estrutura de Dados;
Sistemas Operacionais;
Programação Orientada a Objetos;
Engenharia de Software;
Banco de Dados;
Redes de Computadores;
Segurança da Informação;
Programação Web;
Programação para dispositivos móveis;
Inteligência Artificial e Ciência de Dados.

### PROGRAMAÇÃO ORIENTADA A OBJETOS

#### MÉTODOS ESTÁTICOS

Métodos que pertencem a classe, e não ao objeto.
Podem ser chamados sem instanciar.
Não podem ser alterados por sobrescrita(polimorfismo)

#### ENCAPSULAMENTO

Encapsulamento estrito - os atributos são realmente privados, não dá pra acessar
de fora da classe, apenas indiretamente por meio de get e set. 
Python não tem essa funcionalidade, Java possui.

~~~
class Pessoa:
    def __init__(self):
            self.__idade = 18
~~~

Nesse exemplo nada impede que alguém faça:

~~~
p.Pessoa__idade
~~~

Agora se for em Java:

~~~
{ private int idade;} //dentro da classe

p.idade //fora da classe gera um erro de compilação
~~~

#### ABSTRAÇÃO

(IFPA-2024) Classes abstratas não podem ser instanciadas, elas apenas são uma base que devem
ser herdadas por classes que serão instanciadas.

Elas permitem herança múltipla(IFES-2024)? Python e C++ permitem, Java e C# não.

Uma subclasse de uma classe abstrata só será ***concreta(instanciável)*** se implementar todos
os métodos abstratos herdados.

#### POLIMORFISMO

Permite a redefinição de métodos estáticos(IFES-2024)? Não! [métodos
estáticos](#metodos-estaticos)

### ALGORITMOS E ESTRUTURAS DE DADOS    

#### ESTRUTURAS HETEROGÊNEAS X HOMOGÊNEAS

(IFMT-2023) Quando a estrutura de dados possui campos com tipos distintos dizemos que ela é
heterogênea. Exemplo:

~~~

tipo

BIMESTRE = conjunto[1..4] de real

CAD_ALUNO = registro
                NOME: caractere
                NOTA: BIMESTRE
            fim_registro

var
    ALUNO: conjunto[1..8] de CAD_ALUNO

~~~

#### FILAS

FIFO(First In First Out) ou PEPS(Primeiro a Entrar Primeiro a Sair).


#### ARVORE BINÁRIA

(IFPI-2022) Percorrerendo os nós de uma árvore binária:

~~~
      60
     /   \
   10     20
   /     /  \
  50    100  30
  /\      \    \ 
90  80    70    40
~~~

Pré-ordem(normal -> raiz esquerda direita): 60 10 50 90 80  20  100 70 30 40

Pré-ordem(inversa-> raiz direita esquerda): 60 20 30 40 100 70  10  50 80 90

Em-Ordem(normal  -> esquerda raiz direita): 90 50 80 10 60  100 70  20 30 40 

Em-Ordem(inversa -> direita raiz esquerda): 40 30 20 70 100 60  10  80 50 90  

Pós-Ordem(normal -> esquerda direita raiz): 90 80 50 10  70 100 40  30 20 60 

Pós-Ordem(inversa-> direita esquerda raiz): 40 30 70 100 20 80  90  50 10 60


Questão(IFPA-2022):

~~~
    8
   / \
  4   9
 / \
3   6
   /
  5
~~~

pré-ordem(pré-fixado): 8 4 3 6 5 9
ordem(in-ordem): 3 4 5 6 8 9
pós-ordem(pós-fixado): 3 5 6 4 9 8
 

#### PORTUGUÊS ESTRUTURADO

#### MATRIZES

