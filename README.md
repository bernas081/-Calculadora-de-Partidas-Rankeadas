# 🏆 Calculadora de Partidas Ranqueadas

Projeto desenvolvido como parte de um desafio da **DIO (Digital Innovation One)**, com o objetivo de praticar os fundamentos da lógica de programação utilizando **JavaScript**.

---

## 📌 Descrição do Desafio

Criar uma função que receba como parâmetro a quantidade de **vitórias** e **derrotas** de um jogador e:

- Calcule o **saldo de vitórias** (`vitórias - derrotas`)
- Determine o **nível do jogador** com base no número de vitórias
- Exiba uma mensagem final informando o saldo e o nível alcançado

---

## 🛠️ Tecnologias Utilizadas

- JavaScript (ES6)
- Node.js (opcional para execução)
- Git & GitHub

---

## 📚 Conceitos Aplicados

- Variáveis
- Operadores
- Funções
- Estruturas de decisão (`if / else`)
- Boas práticas de organização de código

---

## 🧮 Regras de Classificação

| Vitórias | Nível |
|--------|--------|
| Menor que 10 | Ferro |
| 11 a 20 | Bronze |
| 21 a 50 | Prata |
| 51 a 80 | Ouro |
| 81 a 90 | Diamante |
| 91 a 100 | Lendário |
| 101 ou mais | Imortal |

---

## 💻 Código Principal

```javascript
function calcularRank(vitorias, derrotas) {
  let saldoVitorias = vitorias - derrotas;
  let nivel = "";

  if (vitorias < 10) {
    nivel = "Ferro";
  } else if (vitorias >= 11 && vitorias <= 20) {
    nivel = "Bronze";
  } else if (vitorias >= 21 && vitorias <= 50) {
    nivel = "Prata";
  } else if (vitorias >= 51 && vitorias <= 80) {
    nivel = "Ouro";
  } else if (vitorias >= 81 && vitorias <= 90) {
    nivel = "Diamante";
  } else if (vitorias >= 91 && vitorias <= 100) {
    nivel = "Lendário";
  } else {
    nivel = "Imortal";
  }

  return `O Herói tem de saldo de ${saldoVitorias} está no nível de ${nivel}`;
}

// Exemplo de uso:
let resultado = calcularRank(75, 20);
console.log(resultado);


//Feito por: Bernardo Sobral de Melo


🚀 Autor

Projeto desenvolvido por Bernas
Desafio proposto pela Digital Innovation One (DIO) 💙
