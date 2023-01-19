# Teste Full Stack(Laravel/Vue) - Lista de Carros

## Objetivo:

Este teste possui como objetivo simular o financiamento de um veículo no qual o
cliente possui interesse. Seguindo o layout proposto [neste link](https://www.figma.com/file/jskUj0P6u57h6kSSAWoFWZ/Teste-Full?node-id=0%3A1&t=LJ83QiUenke6oTY1-0).

Para que esse requisito seja atendido, deverá ser criado um banco de dados, com uma
tabela de veículos, no qual ela deverá armazenar um código id, foto, cidade, marca, modelo,
descrição, ano, quilometragem, tipo de câmbio, telefone da loja e valor do veículo.
Para fins de testes, esta tabela deverá ser popular com alguns registros.
Para esta aplicação será necessário a utilização do framework Laravel para o backend,
VueJS para o frontend e banco de dados MySQL.

## Requisitos do Sistema:
1. O sistema deve permitir que o cliente selecione qual veículo deseja simular o
financiamento;
2. Ao selecionar o item, o sistema deve exibir o valor do veículo selecionado e um
campo para que ele coloque o valor de entrada que deseja dar no financiamento;
   * A: O valor de entrada, pode ser qualquer valor inferior ao veículo que esteja
sendo simulado.

1. Ao clicar em simular o sistema deve exibir os valores das parcelas simuladas.
   * A: A fórmula para calcular as parcelas é: (valor do carro - valor da entrada) /
números de parcelas;
   * B. O valor do carro deve ser calculado com base no número de parcelas que o
cliente optar, seguindo as seguintes regras:
     * i.
Para parcelamento em 6 meses, deve ser considerado um
crescimento de 12.47% no valor total do veículo;
     * ii.
Para parcelamento em 12 meses, deve ser considerado um
crescimento de 15.56% no valor total do veículo;
     * iii.
Para parcelamento em 48 meses, deve ser considerado um
crescimento de 18.69% no valor total do veículo;

## Recursos desejáveis:

4. Utilização do VueX para gerenciar os (estado) state da aplicação;
5. Utilização de recurso de cache em requisições backend;
6. Ambiente de desenvolvimento em Docker.