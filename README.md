# 🗺️ API de Cidades e Estados Brasileiros 🇧🇷

<p align="center">
  <img src="https://img.shields.io/badge/NODE.JS-v18+-green?style=for-the-badge&logo=node.js" />
  <img src="https://img.shields.io/badge/JAVASCRIPT-ES6+-yellow?style=for-the-badge&logo=javascript" />
  <img src="https://img.shields.io/badge/STATUS-OPERACIONAL-blue?style=for-the-badge&logo=serverfault" />
</p>

---

## 🚀 Sobre o Projeto

Esta é uma biblioteca de processamento de dados geográficos do Brasil. Ela foi projetada para filtrar e estruturar informações sobre estados, capitais, regiões e cidades de forma rápida e eficiente. ⚡

### 📂 Estrutura de Arquivos

* **`/modulo`**: O coração do projeto! ❤️
    * `estados.js`: Contém o JSON massivo com todos os dados.
    * `funcoes.js`: Contém a inteligência da API (os filtros).

---

## 🛠️ Funcionalidades (Endpoints de Lógica)

Aqui estão as ferramentas que você pode usar para minerar os dados:

| Função | O que ela entrega? | 🎁 |
| :--- | :--- | :---: |
| `getListaDeEstado` | Sigla, nome e capital de um estado específico. | 📍 |
| `getDadosEstado` | Lista completa de todas as cidades de um estado. | 🏙️ |
| `getCapitalEstado` | A capital de um estado a partir da sigla. | 🏛️ |
| `getEstadosRegiao` | Agrupa todos os estados de uma região (ex: Sul, Norte). | 🗺️ |
| `getCapitalPais` | Informações sobre as capitais históricas do Brasil. | 👑 |
| `getCidades` | Retorna o array puro de nomes de cidades de uma UF. | 📝 |

---

## 🕹️ Como Rodar a Engrenagem

Para utilizar as funções em seu arquivo principal (`app.js`), siga o modelo abaixo:

```javascript
// 📦 Importando a inteligência do projeto
const { getListaDeEstado, getEstadosRegiao } = require('./modulo/funcoes.js');
const { estadosCidades } = require('./modulo/estados.js');

// 🔍 Exemplo: Buscando estados do Sudeste
const resultado = getEstadosRegiao(estadosCidades, 'Sudeste');

console.log(resultado);
🌈 Visualizando o Retorno (JSON)
Quando você busca por uma região, a mágica acontece assim: ✨

JSON
{
  "regiao": "SUL",
  "estados": [
    { "uf": "PR", "descricao": "Paraná" },
    { "uf": "RS", "descricao": "Rio Grande do Sul" },
    { "uf": "SC", "descricao": "Santa Catarina" }
  ]
}

```

👨‍💻 Desenvolvedor
<table style="border: none;">
<tr>
<td align="center">
<a href="#">
<img src="https://github.com/alvesthzin-art.png" width="100px;" alt="Avatar"/><br />
<sub><b>@alvesthzin-art</b></sub>
</a>
</td>
</tr>
</table>
