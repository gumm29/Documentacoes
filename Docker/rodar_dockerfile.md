Para rodar um dockerfile

```bash
docker build -t nomeDaImage .
```

Exemplo de dockerfile
```bash
version: '3'
services:
  teste:
    image: teste
    ports:
      - 80:80
```

Para visualizar container rodando
```bash
docker container ls
```

Rodar docker-compose.yml quando se esta no mesmo diretório
```bash
docker-compose up
```
