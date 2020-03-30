# AULA 01
- Dicas: 
    - [Cheatsheet de como editar um arquivo markdown]
    - Atalhos uteis do teclado
        |Função          |FireFox      |Chrome       |
        |----------------|-------------|-------------|
        |Abrir o console |Ctrl+Shift+K |Ctrl+Shift+J |
        |Limpar console  |Ctrl+Shift+L |Ctrl+L       |

---
### Desafio
No final da aula foi proposto o desafio de calcular, aproximadamente, quantas vezes nosso coração já bateu.<br>
Na própria página da [primeira aula] estão as informações de como poderiamos realizar essa conta.

> Calculo das batidas
> 
> O nosso coração bate uma média de 75 vezes por minuto aproximadamente. Sabemos que 1 hora tem 60 minutos. Com essa informação conseguimos descobrir quantas batidas por hora o coração dá.
> 
> Agora que sabemos as batidas por hora, conseguimos saber quantas batidas ele da por dia já que sabemos quantas horas tem o dia.
> 
> Com a informação da quantidade de batida que o coração da por dia, conseguimos calcular quantas batidas o coração da por ano já que sabemos quantos dias o ano tem. Agora é só calcular quanto o coração já bateu durante toda nossa vida.

Logo, a conta seria algo do tipo:<br>
`(75 vezes por minuto) x (60 minutos por hora) x (24 horas por dia) x (365 dias por ano) x (minha idade autal)`

Agora, fazendo a tradução disso para javascript e sendo que eu tenho 27 anos:
```javascript
75*60*24*362*27;
```
Obtemos o valor de `1064340000` batimentos.

A fim de praticar o que foi exibido durante a aula e exibindo esse resultado um pouco mais perfumado do que só umas letrinhas no console do navegador, poderiamos:
```javascript
alert(75*60*24*362*27);
```

---
### Solução dos exercícios
#### Exercício 01:
> O Criador de galinha me falou o seguinte: "Comprei 15 galinhas por 300 reias" Quanto ele pagou por cada galinha?
```javascript
alert("O criador pagou " + 300/15 + " reais por galinha.");
```
#### Exercício 02:
> Maria foi a padaria e comprou 19 balas, dpois voltou a padaria e comprou mais 45. Quantas balas Maria tem agora?
```javascript
alert("Maria tem agora " + 19+45 + " balas.");
```

#### Exercício 03:
> Para calcular a área de uma circunferência usamos a seguinte fórmula: area = pi x raio x raio. O valor de pi = 3.14, se o valor do meu raio é 2 qual a área da circunferência?
```javascript
alert("A circunferência possui " + 3.14*(2**2) + " unidades de medida de área");
```
---
Tu deve ter notado que no último exercício em fiz algo diferente.
Matemáticamente, realizar a multiplicação de dois entes iguais é a mesma coisa que elevar aquele ente ao quadrado. 
Realizar a multiplicação de um ente por si mesmo três vezes é a mesma coisa que elevar aquele ente ao cubo. E assim por diante.
O nome disso é [potenciação].<br> Em javascript, realizar essa operação pode ser feita utilizando o operador `**`, onde o termo que vem antes do operador é a base e o segundo o expoente.
> raio x raio = raio<sup>2</sup> = raio**2

Assim, caso um dia seja preciso calcular algo do tipo 2<sup>8</sup>, ao invés de escrever no código `2*2*2*2*2*2*2*2` poderiamos fazer simplesmente `2**8`!

---
<a href="https://github.com/Holzlsauer">
    <img src="https://image.flaticon.com/icons/svg/25/25231.svg" width="30" title="Holzlsauer's github">
</a>
<a href="https://en.wikipedia.org/wiki/Creative_Commons_license">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Cc-by-nc-sa_icon.svg/88px-Cc-by-nc-sa_icon.svg.png" title="Creative Commons">
</a>





[Cheatsheet de como editar um arquivo markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[primeira aula]: https://www.alura.com.br/quarentenadev/aula01-javascript
[potenciação]: https://pt.wikipedia.org/wiki/Exponencia%C3%A7%C3%A3o
[cc]: https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Cc-by-nc-sa_icon.svg/88px-Cc-by-nc-sa_icon.svg.png
