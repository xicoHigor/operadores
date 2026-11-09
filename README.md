# Dashboard de Operadores — Loja 01

Dashboard interativo para acompanhar o desempenho de vendas por operador da Loja 01. O painel reúne indicadores individuais, projeção de vendas para o fim do mês e um ranking comparativo.

## Funcionalidades

- Indicadores de venda realizada, média diária, projeção mensal, percentual da meta, ritmo necessário para atingir a meta e participação na loja.
- Comparação visual entre a projeção de cada operador e a meta mensal.
- Ranking com ordenação por venda, média diária, clientes, ticket, participação e projeção.
- Seleção de operadores pelo menu, pelas setas, pelo gráfico ou pela tabela.
- Layout responsivo para telas menores.

## Tecnologias

- HTML
- CSS
- JavaScript
- SVG para o medidor visual

O dashboard é um arquivo estático e não depende de instalação de bibliotecas ou servidor.

## Como visualizar

1. Baixe ou clone este repositório.
2. Abra o arquivo HTML em um navegador atualizado.
3. Selecione um operador para ver os indicadores individuais. Clique nos títulos das colunas do ranking para ordenar os resultados.

Para publicar o painel com GitHub Pages, coloque o arquivo HTML na raiz do repositório e habilite o Pages nas configurações do GitHub. O endereço publicado abrirá o dashboard diretamente.

## Indicadores e período

A versão atual do arquivo apresenta dados de **01/11 a 08/11/2026**, com uma meta mensal de **R$ 120.000**. A projeção segue esta regra:

```text
Projeção mensal = (venda líquida realizada ÷ dias realizados) × dias do mês
```

O ritmo diário necessário considera o valor que falta para a meta dividido pelos dias restantes. A média pode ficar abaixo do real para operadores que não trabalharam todos os dias do período considerado.

## Atualização dos dados

Os dados estão definidos diretamente no JavaScript do HTML. Para atualizar o painel:

1. Atualize o array `OPS` com os dados dos operadores.
2. Atualize a constante `META` se a meta mensal mudar.
3. Atualize o período e os dados gerais exibidos no subtítulo do cabeçalho.
4. Revise os números de dias usados nos cálculos de projeção, pace e ritmo diário para que correspondam ao novo período.

## Privacidade

Antes de publicar o repositório como público, confirme que os nomes, códigos e resultados individuais dos operadores podem ser divulgados. Se necessário, anonimize os dados no array `OPS`.
