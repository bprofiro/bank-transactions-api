<div align="center"> 
  <img src="https://camo.githubusercontent.com/8c13dc2618dbd7f76d1d574350b98fdee1335ce5/68747470733a2f2f726f636b6574736561742d63646e2e73332d73612d656173742d312e616d617a6f6e6177732e636f6d2f626f6f7463616d702d6865616465722e706e67" />
 </div>
 
<h3 align="center">
  Challenge 02: First Node.js project
</h3>


<p align="center">
   <img src="https://github.com/bprofiro/assets/blob/master/node.png" />
</p>

<div>
  <h2> :rocket: About the challenge: </h2>
  
  

  - **`POST /transactions`**: The route must receive `title`,` value` and `type` within the body of the request, with` type` being the type of the transaction, which should be `income` for incoming (deposits) and` outcome` for exiting (withdrawn) . When registering a new transaction, it will be stored inside an object with the format like the following:

```json
{
  "id": "uuid",
  "title": "Salário",
  "value": 3000,
  "type": "income"
}
```

- **`GET /transactions`**: This route will return a listing with all the transactions you have registered so far, together with the sum of the entries, withdrawals and total credit. This route will return an object with the following format:

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
  <h2> :computer: Techs: </h2>
   <p> This project was built in just one language: JavaScript, using the following technologies:

   -   [Node.js](https://nodejs.org/en/)
  </p>
</div>
