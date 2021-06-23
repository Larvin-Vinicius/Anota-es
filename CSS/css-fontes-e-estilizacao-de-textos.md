# FONTES

As propriedades responsáveis por estiliar os textos no css são divididas em duas categorias:

* Baseadas em fonte
	* iniciam com font-*
* Baseadas em texto
	* iniciam com text-*


## Font Family

Declara qual fonte vai ser utilizada e qual a fonte substituta caso a fonte utilizada não esteja disponivel.
Seus valores com as fontes escolhidas são separados por virgula.

```css
p {
	font-family: fonte-principal, fonte-secundaria, fonte-secundaria2 ...;
}

```

* As fontes substitutas são escolhidas na ordem da inserção.
* Geralmente a ultima fonte é um tipo especifico que utilizara a fonte padrão do sistema
	* comumente sans-serif ou serif.

```css

body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}

```

## Font Size

* `font-size`

Altera o tamanho da fonte utilizando um valor de comprimento do css(pixel, em e etc)

```css

body {
  font-size: 14px;
}

```

## Font Style

* `font-style`

Define um estilo ao texto com quatro possiveis valores: italic, normal, inherit e oblique.
Os mais utilizados são: normal e italic

```css

.special {
  font-style: italic;
}

```

## Font Weight

* `font-weight`

Altera a largura da letra e pode aplicar a caracteristica de negrito, a propriedade aceita valores numericos ou quatro valores especificos: normal, bold, bolder, lighter e inherit;

* É recomendados utilizar: bold e normal
	* Bold para negrito
	* Normal para remover o negrito

Em caso de espessuras mas largas que o negrito e mais finas que o normal é recomendado utiliza valores numericos para melhor controle.

```css

p {
	font-weight: bold;

}
```

Os valores numéricos são classificados em centenas de 100 a 900 (100, 200, 300...)
onde o 100 é o mais fino e o 900 o mais espesso.

Para referencia:

* `font-weight: normal` = 400
* `font-weight: bold` = 700

## Line Height

* `line-height`

Define a altura da linha de um texto utilizando valoes de comprimento do css. Uma pratica recomendada é utilizar 150% ou 1.5 que define 1.5 x maior que a fonte atual. Para melhor controle utilize os pixels.

* Também pode ser utilizada para centralizar verticalmente uma unica linha de texto definindo um valor para line-height e para height iguais

```CSS
.btn {
  height: 22px;
  line-height: 22px;
}
```

## Abreviandos as propriedades de fonte

* `font`

Na seguinte ordem:

`font: font-style, font-variant, font-weight, font-size, line-height, font-family.`

* Os valores  de font-family devem ser separados por virgula
* `font-size` e `line-height` deve ser separado por \

```css
html {
  font: italic small-caps bold 14px/22px "Helvetica Neue", Helvetica, Arial, sans-serif;
}
```


