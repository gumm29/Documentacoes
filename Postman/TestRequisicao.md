Para criar uma requisicao com dados de payload personalizados, basta seguir o padrao:

```javascript
pm.test('teste de request', ()=>{
    var options = {
        url: 'https://api.github.com/projects/columns/18980000/cards',
        method: 'POST',
        header: {'Accept': 'application/vnd.github+json',
        'Authorization': 'token IJSY_Wb8K7ZBUGjsPlP3ZjC0lmMejV9IJIJ&K92T',
        'Content-Type': 'application/json'},
        body: '{ "note": "this is json teste" }'
    }

    pm.sendRequest(options, (err, res) => console.log(res))
    pm.response.to.have.status(201);
})
```
