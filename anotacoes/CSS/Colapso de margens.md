O colapso de margens acontece quando as margens de elementos encostam uma na outra. O comportamento que seria esperado era que as margens somassem seus tamanhos.

A partir do momento que as margens se tocam, a margem valida sempre será a de maior numero, anulando totalmente a de menor numero e caso tenha os valores iguais o valor da margem será este valor.

**Condições para o recolhimento da margem**:

-   elemento do tipo **block**
-   Só acontece verticalmente

**Condições para o não recolhimento da margem**:

-   Elemento com display flex
-   Elemento com display grid
-   Elemento com position aplicado.

**Exemplo**:

```css
body {
    margin-top: 5px;
   /* margem será colapsada pois é menor que a margin do elemento filho */
}

div {
    margin-top: 10px;
    margin-bottom: 10px;
   /* margem será colapsada pois é igual a margin do elemento acima */
}

p {
    margin-top: 9px;
    /* margem será colapsada pois é menor que a margin do elemento acima */
}
```

## Quando os recolhimentos de margem ocorrem.

Margem do elemento pai e filho se tocam. Margem superior do pai com a do filho e margem inferior do pai com a do filho.

![coplapso-de-margens-pai-e-filho-top-bottom.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4df79ad8-cbd5-479a-a77f-c95ac3dc5e9b/coplapso-de-margens-pai-e-filho-top-bottom.png)

![coplapso-de-margens-pai-e-filho-top-bottom-2.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0cd0a16d-8dcd-4010-ae17-69e31d5b2121/coplapso-de-margens-pai-e-filho-top-bottom-2.png)

Entre elementos “irmãos”, quando a margem inferior de um e superior do outro se tocam.

![coplapso-de-margens-irmaos.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a3ca524c-0b7f-4df6-83e3-6523e588bedb/coplapso-de-margens-irmaos.png)

Quando o elemento não tem altura, as suas margens inferior e superior somem.

![coplapso-de-margens sem altura.png](https://github.com/Larvin-Vinicius/Notas/blob/main/imagens/coplapso-de-margens%20sem%20altura.png?raw=true)

### Como evitar o colapso entre elementos pai e filho.

-   Utilizar uma borda no elemento pai
    
-   Aplicar um _**padding**_ no elemento pai
    
-   Referências
    
    [What's the Deal with Collapsible Margins?](https://bitsofco.de/collapsible-margins/)
    
    [What's the Deal with Margin Collapse? | Jonathan Harrell](https://www.jonathan-harrell.com/blog/what%E2%80%99s-the-deal-with-margin-collapse/)
    
    [What You Should Know About Collapsing Margins | CSS-Tricks](https://css-tricks.com/what-you-should-know-about-collapsing-margins/)