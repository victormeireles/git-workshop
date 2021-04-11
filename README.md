# Comandos básicos:

Vamos supor que eu quero guardar no meu projeto todas as receitas da minha família.
Inicialmente eu já tenho algumas receitas que adicionei anteriormente.

01. Crie um arquivo bolo-de-laranja.txt de receita nova de bolo de laranja com o texto indicado abaixo:

```
INGREDIENTES
4 ovos
2 xícaras (chá) de açúcar
1 xícara (chá) de óleo
suco de 2 laranjas
casca de 1 laranja
2 xícaras (chá) de farinha de trigo
1 colher (sopa) de fermento

MODO DE PREPARO
Bata no liquidificador os ovos, o açúcar, o óleo, o suco e a casca da laranja.
Passe para uma tigela e acrescente a farinha de trigo e o fermento.
Leve para assar em uma forma com furo central, untada e enfarinhada, por mais ou menos 30 minutos.
Desenforme o bolo e molhe com suco de laranja.
```

02. Agora, vamos editar uma das receitas que já tínhamos anteriormente: strogonoff.txt

03. Se você digitar `git status` você verá o arquivo bolo-de-laranja.txt em untracked files e strogonoff.txt em modified. Adicione estes arquivos para staged: `git add .`
Agora, se você checar `git status` novamente, ambos os arquivos estarão em verde, dentro de changes to be commited. Isso significa que ambos estão em staged :)

04. Agora vamos salvar nossas alterações no git, ouse seja, em um commit:
`git commit -m "<mensagem do commit>"`
Na mensagem do commit coloque um texto que esclareça as mudanças feitas. Pode algo na linha: `feat: adding new receip of orange cake | fix: fixing strogonoff receipt`

05. Temos uma receita que não quero mais ter no meu projeto: 'sopa-de-legumes.txt'. Entretanto eu quero mantê-la no meu local:
`git rm --cached sopa-de-legumes.txt`
Agora, checkando novamente `git status`, este arquivo está nos untracked files.
Como eu commito sem o git reclamar que eu não estou adicionando este arquivo que está untracked??

Vamos adicionar um arquivo chamado .gitignore e coloar o nome do arquivo que eu quero ter no meu local, mas não na nuvem (sopa-de-legumes.txt)
Se checkarmos o git status novamente, este arquivo não está mais em untracked, só precisamos adicionar o .gitgnore

`git add .`
`git commit -m "fix: removing sopa-de-legumes.txt"`

06. Por fim, vamos jogar todas as alterações na nuvem com o push:
`git push -u origin 01-comandos-basicos`