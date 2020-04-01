# AULA 03
- Dicas: 
    - [Como eu editei esse markdown]
    - Atalhos úteis do teclado
        |Função          |FireFox      |Chrome       |
        |----------------|-------------|-------------|
        |Abrir o console |Ctrl+Shift+K |Ctrl+Shift+J |
        |Limpar console  |Ctrl+Shift+L |Ctrl+L       |
        
     - [Artigo] de como funciona e como configurar o [codepen.io]

---
### Apresentando o codepen.io
Durante a [terceira aula] da #QuarentenaDev foi apresentada a página [codepen.io], que funciona como um ambiente de desenvolvimento Front-End com HTML, CSS e o que queremos, Javascript.<br>
Assim como nas anteriores, foram propostos exercícios no final da aula para auxiliar na fixação do conteúdo.

#### Exercício 01:
> Consegue fazer o texto abaixo aparecer na tela?
> ```
> Oi
> como
> você
> está
> pulando
> linha
> ?
> ```

Inicialmente pensei em resolver esse exercício utilizando [escape character], que nada mais são do que um conjunto de dois ou mais caracteres que executam uma certa funcionalidade quando inseridos no meio de um texto no programa.<br>
Neste caso o que seria utilizado é o `\n`, que possuí a função de "pular uma linha". Onde ele aparecer, o programa irá entender que é para ele dar um "Enter" e continuar seja lá o que vier depois.
```javascript
document.write('Oi\ncomo\nvocê\nestá\npulando\nlinha\n?')
```
Porém foi exibido na tela o que foi escrito, **'Oi\ncomo\nvocê\nestá\npulando\nlinha\n?'**. Por que isso?<br>
Assim como foi dito na [segunda aula], a função `document.write()` serve para escrever sobre "a página" que é escrita em **HTML**, cujo o comando usado para pular linha é o `<br>`.

Com isso em mente, a solução correta do exercício seria:
```javascript
document.write('Oi<br>como<br>você<br>está<br>pulando<br>linha<br>?')
```
Que pode ser conferida no [codepen].

#### Exercício 02:
> O carro da Amanda faz 12km/l, ela viajou por 10 horas a uma velocidade de 81km/h. Quantos de litros combustível foram necessários para realizar essa viagem?

Primeiro, para sabermos quantos litros a Amanda utilizou precisamos saber o total de kilometros que foram percorridos, já que sabemos o quanto ela gasta **a cada kilometro**.<br>
Sabendo também que ela percorre um total de 81km **a cada hora** da viagem, e que ela durou 10 horas. O total de kilometros percorrido é:
```
Total = 81km/h x 10h
```

E assim, o total de combustível gasto:
```
Combustível = Total / 12km/l
```

Passando tudo isso para código, teremos:
```javascript
total = 81*10
combustivel = total/12
document.write('Amanda precisou de ' + combustivel + ' litros de combustivel.')
```

Cuja solução também pode ser vista [aqui].

---
### Sobre o exercício 01
Então a minha primeira ideia para a solução para o exercício 01 estava errada?<br>
Não totalmente. Na maioria das linguagens são utilizados os [escape character] para algumas funções, o que inclui o **new line**. Mas como o texto estava sendo escrito em um **documento html** e nessa linguagem a quebra de linha é feita de forma diferente, o resultado foi de fato diferente do desejado.<br>
Agora, e se o lugar onde fosse ser escrito aqueles texto utilizando o `\n` o compreendesse, teríamos o texto de saída como desejado. E um lugar que entende esse caracteres é o **console**.<br>
Para escrever no console do navegador o comando utilizado é o `console.log()`, de forma que executando o comando abaixo e abrindo o console do navegar podemos ver o texto como é desejado pelo exercício.
```javascript
console.log('Oi\ncomo\nvocê\nestá\npulando\nlinha\n?')
```
[Resposta no codepen]



---
<a href="https://github.com/Holzlsauer">
    <img src="https://image.flaticon.com/icons/svg/25/25231.svg" width="30" title="Holzlsauer's github">
</a>
<a href="https://en.wikipedia.org/wiki/Creative_Commons_license">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Cc-by-nc-sa_icon.svg/88px-Cc-by-nc-sa_icon.svg.png" title="Creative Commons">
</a>





[Como eu editei esse markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[Artigo]: https://www.alura.com.br/artigos/codepen-o-que-e-e-como-usar
[codepen.io]: https://codepen.io/
[terceira aula]: https://www.alura.com.br/quarentenadev/aula03-codepen
[escape character]: https://en.wikipedia.org/wiki/Escape_character
[segunda aula]: https://www.alura.com.br/quarentenadev/aula02-variaveis
[codepen]: https://codepen.io/Holzlsauer/pen/rNVbxEe
[aqui]: https://codepen.io/Holzlsauer/pen/bGdJpVy
[Resposta no codepen]: https://codepen.io/Holzlsauer/pen/yLNrOzJ
[cc]: https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Cc-by-nc-sa_icon.svg/88px-Cc-by-nc-sa_icon.svg.png
