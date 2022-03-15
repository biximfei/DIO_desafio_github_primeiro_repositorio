# JAVASCRIPT

## **Boas Práticas**
___
- Externar o código: _Colocar o código em um arquivo .js e fazer o link usando a tag \<script src="caminho/arquivo.js">\</script>_
- Introduzir o link do código antes do fechamento da tag body _(\</body>)_
- Declarar as variaveis e as constantes no topo do código;
- Utilizar, preferencialmente, o **let** para declerar variáveis;
- Declarar variávei usando o formato _camelCase ou \_ : _var nomeCompleto ou var nome_completo;_
- Declarar constantes com letras maiúsculas: _const ANO_DE_CRIACAO;_

<br />

## **Lembretes**
___
### **Comandos para criar variáveis e constantes**
- var – _escopo global e local, pode ter seu valor alterado, se não
tiver um valor inicial será tratada como null;_
- let – _escopo local de bloco, pode ter seu valor alterado, se não
tiver um valor inicial será tratada como null;_
- const – _escopo local de bloco, somente leitura, o valor inicial é
obrigatório e não pode ser alterado._

### **Manipuladores de arrays**
- _forEach() – itera um array;_
- _push() – add item no final do array;_
- _pop() – remove item no final do array;_
- _shift() – remove item no início do array;_
- _unshift() – add item no início do array;_
- _indexOf() – retorna o índice de um valor;_
- _splice() – remove ou substitui um item pelo índice;_
- _slice() – retorna uma parte de um array existente;_

### **Operadores Aritiméticos**
- **\+** _adição;_
- **\-** _subtração;_
- **\*** _multiplicação;_
- **\/** _divisão real;_
- **\%** _divisão inteira;_
- **\*\*** _potenciação;_

### **Operadores Relacionais**
- **\=\=**  - valores tipo numéricos são iguais aos seus valores tipo string _("0" \=\= 0)=\>true;_
- **\=\=\=** - valores e tipos tem que serem iguais _("0" \=\= 0)=\>false;_
- **\>**    - maior que;
- **\<**    - menor que;
- **\>\=**  - maior ou igual a;
- **\<\=**  - menor ou igual a;

### **Operadores Lógicos**
- **&&** - “e” – considera que todos os valores sejam true;
- **||** - “ou” – considera que qualquer valor seja true;
- **!**  - “não” – inverte o valor de true para false ou vice-versa;

### **Estruturas de Condição**
#### **IF**
**1-** **IF ( ) { }**

if ( _condição_ ){
	_se for verdadeira_
}

**2 -** **IF ( ) { } ELSE { }** 

if ( _condição_ ){
	_se for verdadeira_
} else {
	_se for falsa_
}

**3 -** **IF () {} ELSE IF {} ELSE {}** 

if ( _condição 1_ ){ <br />
&nbsp;&nbsp;&nbsp;&nbsp;_se a primeira condição for verdadeira_<br />
} else if ( _condição 2_ ) {<br />
	_se a segunda condição for verdadeira_ <br />
} else if ( _condição n_ ) { <br />
&nbsp;&nbsp;&nbsp;&nbsp; _se a "enésima" condição for verdadeira_ <br />
} else { <br />
&nbsp;&nbsp;&nbsp;&nbsp; _se nenhuma condição for verdadeira_ <br />
} <br />

**4 -**  **IF TERNÁRIO** 

 _condição_  **?**  _se for verdadeira_  **:**  _se for falsa_

<br />

### **SWITCH/CASE - EXEMPLO**

let jogador1 = 0;\
let jogador2 = 0;\
let resultado;

switch ( resultado ) {\
&nbsp;&nbsp;&nbsp;&nbsp;case  _"jogador1"_:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;console.log("Jogador 1 é o vencedor");\
&nbsp;&nbsp;&nbsp;&nbsp;break;\
&nbsp;&nbsp;&nbsp;&nbsp;case _"jogador2"_:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;console.log("Jogador 2 é o vencedor");\
&nbsp;&nbsp;&nbsp;&nbsp;break;\
&nbsp;&nbsp;&nbsp;&nbsp;default:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;console.log("Iiiihhhh! Empataram!!!");\
}

### **LAÇOS DE REPETIÇÃO - EXEMPLOS**
#### **1. FOR**
for (let i = 0 ; i < 10 ; i++){\
&nbsp;&nbsp;&nbsp;&nbsp;console.log("I = " + i);\
}

#### **2. FOR / IN**
_Funciona como uma repetição a partir de uma propriedade:_\
\
var array = ['valor1', 'valor2', 'valor3', 'valor4'];\
\
for (i in array) {\
&nbsp;&nbsp;&nbsp;&nbsp;console.log( "Indice: " + i + " | Valor: " + array[i] );\
}

#### **3. FOR / OF**

_Funciona como uma repetição a partir de um valor:_
\
var array = ['valor1', 'valor2', 'valor3', 'valor4'];\
\
for (i of array) {\
&nbsp;&nbsp;&nbsp;&nbsp;console.log( "Valor: " + i );\
}

_Obs.: O For/of não funciona com objetos pois as propriedades variam, diferentes do índice em um array que sempre serão números inteiros._
<br /><br /><br />

#### **4. WHILE**
_Executa uma instrução “enquanto” determinada condição for verdadeira, a verificação é feita antes da xecução;_

var a = 0;

while (a < 10 ){    \
&nbsp;&nbsp;&nbsp;&nbsp;console.log(a + " < 10");\
&nbsp;&nbsp;&nbsp;&nbsp;a++;\
}
<br /><br /><br />

#### **5. WHILE**
_Executa uma instrução “até que” determinada condição seja falsa, a verificação é feita depois da execução;_

var a = 0;

do {\
&nbsp;&nbsp;&nbsp;&nbsp;a++;\
&nbsp;&nbsp;&nbsp;&nbsp;console.log(a + " <= 10");\
}  while ( a < 10 )

var a = 0;

_Obs.: Sempre será executado uma primeira vez, por ter a condição ao final do código;_

