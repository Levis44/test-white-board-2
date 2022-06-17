## ❓Case para o desafio

O GCB Academy decidiu propor um desafio para o time de desenvolvedores, desenvolver um algorítimo que fosse capaz de juntar em grupos de estudo de 3 devs para que pudessem construir projetos juntos durante um tempo.

Existem algumas especificidades da forma que esse algorítimo deve formar os grupos, são essas:

- Cada grupo de estudo deve conter no máximo 3 pessoas;
- Em cada grupo, é necessário que existam 2 desenvolvedores Front-end e 1 Back-end;
- O grupo deve ser formado pelas pessoas que menos participaram de grupos de estudos;
- O algorítimo deve sortear quantos grupos forem pedidos;
- É necessário pegar aleatoriamente as pessoas para o grupo;
- Uma pessoa, deve ficar no mínimo 2 vezes sem ir para um grupo de estudos;
- Um grupo deve conter no mínimo 2 pessoas de nível D e 1 nível C;
- Gerar os grupos mostrando os 3 participantes de cada e suas respectivas informações.

A sua missão é: Construir um algorítimo que seja capaz de resolver esse problema.

## ➡️ Exemplo

```jsx
const students = [
  { name: "Jonny", times: 0, level: "C", lastTime: 0, area: "BACK" },
  { name: "Maria", times: 0, level: "D", lastTime: 0, area: "BACK" },
  { name: "Selena", times: 0, level: "D", lastTime: 0, area: "BACK" },
  { name: "Mathew", times: 0, level: "D", lastTime: 0, area: "FRONT" },
  { name: "Lucas", times: 0, level: "D", lastTime: 0, area: "FRONT" },
  { name: "Ana", times: 0, level: "C", lastTime: 0, area: "FRONT" },
  { name: "Allan", times: 0, level: "D", lastTime: 0, area: "BACK" },
  { name: "Wilson", times: 0, level: "C", lastTime: 0, area: "FRONT" },
  { name: "Gabriel", times: 0, level: "D", lastTime: 0, area: "FRONT" },
  { name: "Junior", times: 0, level: "C", lastTime: 0, area: "BACK" },
];

// call your function/method
const result = run({ array: students, groups: 5 });

// show result
console.log(result);

// [
//   [
//     { name: "Allan", times: 2, level: "D", lastTime: 2, area: "BACK" },
//     { name: "Selena", times: 2, level: "D", lastTime: 2, area: "BACK" },
//     { name: "Jonny", times: 1, level: "C", lastTime: 0, area: "BACK" },
//   ],
//   [
//     { name: "Maria", times: 2, level: "D", lastTime: 1, area: "BACK" },
//     { name: "Lucas", times: 2, level: "D", lastTime: 1, area: "FRONT" },
//     { name: "Junior", times: 2, level: "C", lastTime: 1, area: "BACK" },
//   ],
//   [
//     { name: "Mathew", times: 1, level: "D", lastTime: 0, area: "FRONT" },
//     { name: "Gabriel", times: 1, level: "D", lastTime: 0, area: "FRONT" },
//     { name: "Ana", times: 1, level: "C", lastTime: 0, area: "FRONT" },
//   ],
//   [
//     { name: "Selena", times: 2, level: "D", lastTime: 2, area: "BACK" },
//     { name: "Allan", times: 2, level: "D", lastTime: 2, area: "BACK" },
//     { name: "Wilson", times: 1, level: "C", lastTime: 2, area: "FRONT" },
//   ],
//   [
//     { name: "Lucas", times: 2, level: "D", lastTime: 1, area: "FRONT" },
//     { name: "Maria", times: 2, level: "D", lastTime: 1, area: "BACK" },
//     { name: "Junior", times: 2, level: "C", lastTime: 1, area: "BACK" },
//   ],
// ];
```

<aside>
💡 Não leve o resultado do exemplo acima como certo, o algorítimo deve sortear aleatoriamente os participantes que menos foram para o grupo de estudos, portanto, nem toda vez o resultado será o mesmo.

</aside>
