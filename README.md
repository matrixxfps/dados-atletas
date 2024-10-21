Projeto de Avaliação de Atletas
Resumo do Projeto
Este projeto consiste em uma aplicação desenvolvida em JavaScript que recebe informações sobre atletas e calcula parâmetros importantes, como a categoria, o Índice de Massa Corporal (IMC), a média das notas e outras informações relevantes. O sistema é destinado a organizadores de competições de ginástica artística e auxilia na avaliação dos atletas.

Introdução
Os organizadores da competição de ginástica artística precisavam de uma solução para calcular e apresentar as informações dos atletas de forma eficiente. A aplicação foi projetada para receber dados como nome, idade, peso, altura e notas de cinco jurados, e retornar a categoria do atleta, seu IMC e a média válida das notas.

Funcionalidades
A aplicação possui as seguintes funcionalidades:

Recebe dados de um atleta, incluindo:

Nome
Idade
Peso
Altura
Notas dos jurados
Calcula a categoria do atleta com base na idade:

Infantil: 9 a 11 anos
Juvenil: 12 e 13 anos
Intermediário: 14 e 15 anos
Adulto: 16 a 30 anos
Sem categoria: demais idades
Calcula o IMC do atleta utilizando a fórmula:

IMC
=
peso
(
altura
×
altura
)
IMC= 
(altura×altura)
peso
​
 
Calcula a média válida das notas, desconsiderando a maior e a menor nota.

Exibe todas as informações calculadas para o usuário.

Estrutura do Código
A classe Atleta contém os seguintes métodos:

Construtor: Recebe as informações do atleta e inicializa as propriedades.
calculaCategoria(): Retorna a categoria do atleta com base na idade.
calculaIMC(): Retorna o IMC do atleta.
calculaMediaValida(): Retorna a média válida das notas do atleta.
Métodos de Acesso: Permitem acessar as informações do atleta, como nome, idade, peso, notas, categoria, IMC e média válida.
Exemplo de Uso
Aqui está um exemplo de como instanciar a classe Atleta e exibir as informações no console:

javascript

const atleta = new Atleta("Cesar Abascal", 30, 80, 1.70, [10, 9.34, 8.42, 10, 7.88]);

console.log(`Nome: ${atleta.obtemNomeAtleta()}`);
console.log(`Idade: ${atleta.obtemIdadeAtleta()}`);
console.log(`Peso: ${atleta.obtemPesoAtleta()}`);
console.log(`Altura: ${atleta.obtemAlturaAtleta()}`);
console.log(`Notas: ${atleta.obtemNotasAtleta().join(',')}`);
console.log(`Categoria: ${atleta.obtemCategoria()}`);
console.log(`IMC: ${atleta.obtemIMC()}`);
console.log(`Média válida: ${atleta.obtemMediaValida()}`);
Considerações Finais
A aplicação pode ser expandida para incluir mais funcionalidades, como a entrada de dados pelo usuário, manipulação de múltiplos atletas e tratamento de casos de entradas inválidas. O objetivo é fornecer uma ferramenta prática e eficaz para a avaliação de atletas em competições.

Tecnologias Utilizadas
JavaScript: Linguagem de programação utilizada para implementar a lógica da aplicação.
Node.js (opcional): Para executar a aplicação em um ambiente de servidor (caso deseje expandir para uma aplicação web).
Licença
Este projeto é de uso livre. Sinta-se à vontade para modificar e distribuir conforme necessário.

