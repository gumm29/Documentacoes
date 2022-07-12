Exemplo de como pegar resposta de requisicao e gravar em uma variavel de colecao:

```javascript
pm.test('Pegar response e gravar em uma variavel da colecao', ()=>{
  var data = pm.response.json()
  var url = data.url // url eh o campo da resposta do exemplo.  
  pm.collectionVariables.set("variable_key", url);  // variable_key trocar por variavel criada na collection
})
```

Criar mesma variavel 'variable_key' na colecao.
Clique na colection (ou crie uma), va em 'Variables' e em 'key', degite o nome da variavel que deseja (no caso 'variable_key')

Pronto!
Para utilizar a variavel, basta digita-la entre duas chaves {{variable_key}} (o postman ja ira reconhecer, e mostrara um C amarelo - significa que eh uma variavel de colecao)
