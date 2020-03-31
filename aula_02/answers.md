# AULA 02
- Dicas: 
    - [Como eu editei esse markdown]
    - Atalhos úteis do teclado
        |Função          |FireFox      |Chrome       |
        |----------------|-------------|-------------|
        |Abrir o console |Ctrl+Shift+K |Ctrl+Shift+J |
        |Limpar console  |Ctrl+Shift+L |Ctrl+L       |

---
### Três desafios
Na [segunda aula] da **#QuarentenaDev** foram propostos três atividades a fim de reforçar o conteúdo passado em vídeo.

#### Primeiro desafio:
> O IMC ou índice de massa corporal, nos ajuda a identificar algumas caracteristicas como obesidade ou desnutrição. Abaixo temos uma tabela indicando o significado do valor que você encontrar:
> | Valor do IMC      | Categoria            |
> |-------------------|----------------------|
> |Abaixo de 17       | Muito abaixo do peso |
> |Entre 17 e 18,49   | Abaixo do peso       |
> |Entre 18,5 e 24,99 | Peso normal          |
> |Entre 25 e 29,99   | Acima do peso        |
> |Entre 30 e 34,99   | Obesidade I          |
> |Entre 35 e 39,99   | Obesidade II         |
> 
> O IMC é calculado dividindo o peso pela altura elevada ao quadrado. Será que você consegue descobrir qual o seu IMC?
```javascript
peso=prompt("Qual o seu peso?")
altura=prompt("Qual a sua altura?")
document.write('O seu IMC é ' + (peso/altura**2))
```

#### Segundo desafio:
> Guilherme tem 30 anos e tem 3 irmãs, a Carol que tem 20 anos, Márcia que tem 15, Patrícia que tem 10 anos. Qual a média de idade da família do Guilherme?

Para resolver esse desafio eu segui um caminho um pouco diferente. Ao invés de mandar os textos, [strings], como argumentos separados na função `document.write()`, estou mandando apenas uma string apenas, [concatenando] as contas e chamando a função `prompt()` direto com a saída.
```javascript
document.write('A idade média entre Guilherme e suas três irmãs é de ' + (30+20+15+10)/prompt('Quantas pessoas há entre Guilherme e suas irmãs?') + ' anos.')
```

#### Terceiro desafio:
> Quantos anos tem a avó da amiga da Maria que nasceu em 1940?
```javascript
document.write('A avó da amiga da Maria tem ' + (prompt("Em que ano estamos?")-1940) + ' anos.')
```

---
<a href="https://github.com/Holzlsauer">
    <img src="https://image.flaticon.com/icons/svg/25/25231.svg" width="30" title="Holzlsauer's github">
</a>
<a href="https://en.wikipedia.org/wiki/Creative_Commons_license">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Cc-by-nc-sa_icon.svg/88px-Cc-by-nc-sa_icon.svg.png" title="Creative Commons">
</a>





[Como eu editei esse markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[segunda aula]: https://www.alura.com.br/quarentenadev/aula02-variaveis
[strings]: https://pt.wikipedia.org/wiki/Cadeia_de_caracteres
[concatenando]: https://en.wikipedia.org/wiki/Concatenation
[cc]: https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Cc-by-nc-sa_icon.svg/88px-Cc-by-nc-sa_icon.svg.png
