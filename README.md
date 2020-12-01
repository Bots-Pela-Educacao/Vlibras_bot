# Vlibras_bot
Esboço de um projeto com o objetivo de tornar a linguagem de sinais mais 

# links
https://wiki.vlibras.gov.br/

# criar 
- Pacote de figurinhas no telegram com os sinais
- jogo de perguntas
nivel facíl - acertar o nome do sinal com opções
nível médio - acertar o nome do sinal sem opção
nível dificil - acertar o sinal com opções(figurinhas)

- pesquisar sinais inline


# APIs existentes
## pesquisar palavras e retorna um video
processo:

``https://wikiback.vlibras.gov.br/dictionary/1?code=${palavra}``

retorna um aray de resuldados cada um com um ``task_ID`` 

``https://wikiback.vlibras.gov.br/object-task/${task_ID}/2``

retorna um ``path`` para o ``task_ID``

``https://wikiback.vlibras.gov.br/download/${path}``

retorna um video


# API para criar

endpoint: ``/generate/image/pt-libras/${palavra}``

para gerar uma imagem com a sequencia de sinais corespondente a palavra
esse endpoint será usado para o bot criar perguntas ou ensinar soletrar


