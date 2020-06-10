<div align="center"> 
  <img src="https://camo.githubusercontent.com/8c13dc2618dbd7f76d1d574350b98fdee1335ce5/68747470733a2f2f726f636b6574736561742d63646e2e73332d73612d656173742d312e616d617a6f6e6177732e636f6d2f626f6f7463616d702d6865616465722e706e67" />
 </div>
 
<h3 align="center">
  API de Transações Bancárias com Node.JS
</h3>


<p align="center">
   <img src="https://github.com/bprofiro/assets/blob/master/node.png" />
</p>

<div>
  <h2> :rocket: Rotas da API: </h2>
  
  

  - **`POST /transactions`**: A rota deve receber `title`,` value` e `type` dentro do corpo da solicitação, com` type` sendo o tipo da transação, que deve ser `income` para entrada (depósitos) e `outcome` para sair (retirado). Ao registrar uma nova transação, ela será armazenada dentro de um objeto com o formato da seguinte forma:

```json
{
  "id": "uuid",
  "title": "Salário",
  "value": 3000,
  "type": "income"
}
```

- **`GET /transactions`**: Essa rota retornará uma listagem com todas as transações que você registrou até o momento, juntamente com a soma das entradas, saques e crédito total. Esta rota retornará um objeto com o seguinte formato:

```json
{
  "transactions": [
    {
      "id": "uuid",
      "title": "Salário",
      "value": 4000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Freela",
      "value": 2000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Pagamento da fatura",
      "value": 4000,
      "type": "outcome"
    },
    {
      "id": "uuid",
      "title": "Cadeira Gamer",
      "value": 1200,
      "type": "outcome"
    }
  ],
  "balance": {
    "income": 6000,
    "outcome": 5200,
    "total": 800
  }
}
```
</div>

<div>
  <h2> :computer: Tecnologias: </h2>
  <p> Esse projeto foi construído em Node.js e não guarda as informações dentro de um banco de dados. </p>
</div>
