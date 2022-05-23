# PCO102-2022.1

## Problema

O problema a ser abordado nas atividades avaliativas de PCO102 é obter o sentimento geral do publico em relação a filmes brasileiros por gênero(Comédia, aventura, suspense etc.). Esta base pode ser encontrada no Keagle através do link: https://www.kaggle.com/datasets/ashirwadsangwan/imdb-dataset ou no drive através do link: https://drive.google.com/drive/folders/1cV0L-DGcP42SDMSDBL3GLHqKZcQlznc-?usp=sharing

## Base de dados

O conteúdo da base de dados é dividido em 5 arquivos, sendo eles:

### title.akas.tsv.gz - Possúi as seguintes informações para os títulos:
titleId (string) - um tconst, um identificador alfanumérico exclusivo do título. <br />
ordenação (inteiro) – um número para identificar exclusivamente as linhas para um determinado titleId.<br />
title (string) – o título localizado.<br />
region (string) - a região para esta versão do título.<br />
language (string) - o idioma do título.<br />
tipos (array) - Conjunto enumerado de atributos para este título alternativo. Um ou mais dos seguintes: "alternative", "dvd", "festival", "tv", "video", "working", "original", "imdbDisplay". Novos valores podem ser adicionados no futuro sem aviso prévio.<br />
atributos (array) - Termos adicionais para descrever este título alternativo, não enumerados.<br />
isOriginalTitle (booleano) – 0: título não original; 1: título original.<br />

### title.basics.tsv.gz - Possúi as seguintes informações para títulos:
tconst (string) - identificador único alfanumérico do título.<br />
titleType (string) – o tipo/formato do título (por exemplo, filme, curta, série de TV, episódio de TV, vídeo, etc).<br />
primaryTitle (string) – o título mais popular / o título usado pelos cineastas em materiais promocionais no momento do lançamento.<br />
originalTitle (string) - título original, no idioma original.<br />
isAdult (booleano) - 0: título não adulto; 1: título adulto.<br />
startYear (YYYY) – representa o ano de lançamento de um título. No caso de Séries de TV, é o ano de início da série.<br />
endYear (YYYY) – Série de TV final do ano. para todos os outros tipos de títulos.<br />
runtimeMinutes – tempo de execução primário do título, em minutos.<br />
gêneros (array de strings) – inclui até três gêneros associados ao título.<br />

### title.principals.tsv.gz – Possúi o elenco/equipe principal dos títulos:

tconst (string) - identificador único alfanumérico do título.<br />
ordenação (inteiro) – um número para identificar exclusivamente as linhas para um determinado titleId.<br />
nconst (string) - identificador único alfanumérico do nome/pessoa.<br />
categoria (string) - a categoria de trabalho em que a pessoa estava.<br />
job (string) - o título do trabalho específico, se aplicável, senão.<br />
caracteres (string) - o nome do personagem reproduzido, se aplicável, senão.<br />

### title.ratings.tsv.gz – Possúi a classificação do IMDb e informações de votos para os títulos:

tconst (string) - identificador único alfanumérico do título.<br />
averageRating – média ponderada de todas as avaliações de usuários individuais.<br />
numVotes - número de votos que o título recebeu.<br />

### name.basics.tsv.gz – Possúi as seguintes informações para nomes:

nconst (string) - identificador único alfanumérico do nome/pessoa.<br />
primaryName (string)– nome pelo qual a pessoa é mais frequentemente creditada.<br />
birthYear – no formato AAAA.<br />
deathYear – no formato YYYY, se aplicável, senão.<br />
primaryProfession (array de strings) – as 3 principais profissões da pessoa.<br />
knownForTitles (array de tconsts) – títulos pelos quais a pessoa é conhecida.<br />

## Proposta de Solução: 

Eu pretendo solucionar este problema fazendo o uso de ferramentas de machine learning e técnicas de processamento de linguagem natural, para analisar comentários e avaliações sobre os filmes brasileiros e conseguir metrificar o grau de satisfação do público.
