# traducao-automatica
Tente valores diferentes do argumento num_examples na funçãoload_data_nmt. Como isso afeta os tamanhos do vocabulário do idioma de origem e do idioma de destino?

O argumento max_examples limita a quantidade de exemplos utilizados no processo de tokenização, quando um valor menor é definido para max_examples, menos frases são tokenizadas, o que resulta em um vocabulário menor, pois há menos palavras únicas sendo processadas. Conforme aumentamos o valor de max_examples, mais frases são incluídas no processo de tokenização, aumentando o tamanho do vocabulário, já que novas palavras e variações são encontradas.

O texto em alguns idiomas, como chinês e japonês, não tem indicadores de limite de palavras (por exemplo, espaço). A tokenização em nível de palavra ainda é uma boa ideia para esses casos? Por que ou por que não?

Idiomas que não possuem delimitadores claros entre as palavras como espaços em línguas ocidentais, a tokenização por palavras não é a abordagem mais eficiente. Nesses casos, a divisão em palavras pode ser imprecisa, mas existem outro métodos como a tokenização em nível de caracteres ou subpalavras.
