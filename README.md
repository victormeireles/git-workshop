# Merge:

A sua branch master é a '02-merge'. Enquanto você estava desenvolvendo a sua feature, a master também mudou.
Você como um desenvolvedor precavido, vai pegar as útimas mudanças da master para garantir que as suas alterações vão funcionar com o último estado da master :)

01. Altere a receita de strogonoff, de 3 para 5 peitos de frango
02. Adicione, commite e push suas alterações
03. Agora, antes de fazer a sua PR é importante garantir que não haja conflitos. Vamor dar um merge da master na sua branch.

- Como ter certeza que vc está pegando a última versão da master? Você pode dar um checkout e ir pra branch e dar um `git pull` para pegar as últimas alterções ou você pode referciar a master com o prefixo 'origin/', isto garante que você está dando merge com a branch que está na origem (nuvem)
- Na branch 02-merge faça: `git merge 02-master`
- Resolva os conflitos, adicione as mudançar, commite e push :)