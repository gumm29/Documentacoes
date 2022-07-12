Como rodar script do jemter por linha de comando (recomendado pelo jmeter)

Dentro da pasta bin, executar:
```bash
jmeter -n -t caminho/arquivo.jmx -l arquivoResultado.cvs -e -o pastaVaziaParaReport/
```

-n = para rodar apenas pelo terminal

-t = para especificar o arquivo jmx

-l = para especificar onde ficarao os logs (csv ou jtl)

-e = gerar reporte apos o teste //verificar se precisa

-o = pasta onde ira ficar o reporte
