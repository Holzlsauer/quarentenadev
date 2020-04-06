# AULA 04
- Dicas: 
    - [Como eu editei esse markdown]
    - Atalhos úteis do teclado
        |Função          |FireFox      |Chrome       |
        |----------------|-------------|-------------|
        |Abrir o console |Ctrl+Shift+K |Ctrl+Shift+J |
        |Limpar console  |Ctrl+Shift+L |Ctrl+L       |
        
     - [Artigo] de como funciona e como configurar o [codepen.io]

---
### Aplicativo de corrida
Na [quarta aula] da **#QuarentenaDev** foi apresentado o projeto final que será desenvolvido ao longo das aulas, já dando início a ele através de um código para calcular o valor de uma corrida feita por aplicativo.<br>
A fórmula utilizada para o calculo do valor total da corrida consiste em três elementos: um valor fixo, cobrado independentemente do tempo ou distância da corrida; o tempo total gasto na corrida, multiplicado por uma certo taxa; e a distância total percorrida durante a corrida, também multiplicada por uma certa taxa.<br>
Traduzindo:
```
Valor cobrado = 2,00 + (distância em km) x 1,40 + (tempo em minutos) x 0,26
```

Assim, o código final produzido durante a aula foi:
```javascript
distancia = 20
tempo = 60
valor = 2 + distancia*1.4 + tempo*0.26
alert('A corrida ficou em ' + valor.toFixed(2) + 'R$')
```

E assim como foi mencionado durante a aula, o valores decimais são separados por ponto, e não vírgula. Esse separador, apesar de não ser o [padrão SI], é adotado em alguns lugares do mundo, como no Estados Unidos.

#### Exercício
>Na aula a Amanda deixou os valores de distância e tempo fixos no programa. Mas as pessoas querem ir para lugares diferentes certo? Então como deixar as opções de distância e tempo para quem for usar o nosso programa preencher e descobrir o valor da sua corrida? E como mostrar isso na tela sem usar o alert?

Resolver essa atividade pode ser feita utilizando coisas que já foram vistas. A função `prompt()` para receber alguma informação do usuário, e o `document.write()` para exibir o resultado no próprio arquivo da página.
```javascript
distancia = prompt('Qual a distância percorrida, em km?')
tempo = prompt('Qual o tempo da corrida?')
valor = 2 + distancia*1.4 + tempo*0.26

// alert('A corrida ficou em ' + valor.toFixed(2) + 'R$')
document.write('A corrida ficou em ' + valor.toFixed(2) + 'R$')
```
Resultado no [codepen].

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
[quarta aula]: https://www.alura.com.br/quarentenadev/aula04-aplicativo-de-transporte
[padrão SI]: https://en.wikipedia.org/wiki/Decimal_separator#Current_standards
[codepen]: https://codepen.io/Holzlsauer/pen/xxGvgQW
[cc]: https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Cc-by-nc-sa_icon.svg/88px-Cc-by-nc-sa_icon.svg.png
