<img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/logo.png" alt="logo_HDRio" style="zoom:20%;" />

<div align="center">
    <small>Eixo 5 -  Grandes Acervos de Dados Textuais nas Humanidades Digitais</small>
</div>
<div align="center">
    <h1>Por uma Heurística Digital<br>no ofício do Historiador</h1>
</div>

<div align="center">
    <p>  
    <a href="htpps://ericbrasiln.github.io">Eric Brasil</a> (IHL/UNILAB)
    </p>
    <img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/LOGO-HISTÓRIA-BA-novo.png" style="zoom:05%;" /> <img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/unilab.png" style="zoom:25%;" /> <img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/labhd.png" style="zoom:13%;" /></div>

---

:warning: **Disclaimer 1**: *Após um ano de pandemia, tudo mudou no mundo, no Brasil e tb nesse paper. O que inicialmente era uma proposta de reflexão de coleta manual de fontes em um ano se tornou a construção de um programa para raspagem, organização e tabulação dos dados.*
<div align="center">
 <img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/noun_404 Error_1469633.png" style="zoom:30%;" />
</div>


**:warning: Disclaimer 2**: *Desde domingo, 11/04/2021, todos as páginas da Fundação Biblioteca Nacional estão fora do ar!*



<div align="center">
    <blockquote class="twitter-tweet"><p lang="pt" dir="ltr">Por motivos técnicos, nosso site se encontra temporariamente fora do ar. Esperamos solucionar o problema o quanto antes. <a href="https://t.co/OUGMDWE3hJ">pic.twitter.com/OUGMDWE3hJ</a></p>&mdash; Biblioteca Nacional (@FBN) <a href="https://twitter.com/FBN/status/1381632367194963969?ref_src=twsrc%5Etfw">April 12, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
</div>



<br>

---

<br>

## Pesquisa histórica na era da abundância?

<img src="assests/noun_algorithm_3048214.png" style="zoom:30%;" />

- **Digitalização**

- A questão das **ferramentas / métodos X reflexões teóricas e epistemológicas**

- Mas aqui eu gostaria de enfrentar um problema anterior na operação historiográica: o ato de recolher as fontes e organizá-las para efetuar a crítica e posterior análise - a **heurística**. 
  - Para tanto, busco apresentar uma ferramenta de suporte para a coleta de dados no repositório de jornais da BN, a [Hemeroteca Digital Brasileira](http://memoria.bn.br/) e realizar uma breve reflexão sobre as possibilidades para pesquisa.

---

<br>

<br>



## HDB e a noção de *Big Data* para um históriador social
<div align="center">
<img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/noun_Big data_2232102.png" style="zoom:30%;" />
</div>

### Quão grande deve ser o volume de dados para considerarmos *Big Data*?

----

<br>

<br>

### O motor e o reconhecimento:

<img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/noun_Fishing_3839395.png" style="zoom:30%;" />

<br>

> In practice, a full-text search is often a Boolean fishing expedition for a set of documents that may or may not exist. (Underwood, 2014: 64)

---

<br>

HDB foi lançada em 2012 com em torno de 5 milhões de páginas.

- OCR da HDB? ABBYY + DocPro = cadê os dados?
- Dump files com XML, dados de precisão (accuracy), etc

> For historians, the use of search interfaces is essential, but for further digital analysis the material it is necessary to be able to download the data, for example, as a data dump that includes the OCRed texts and metadata, often in international XML standards, such as the METS and ALTO formats. (Salmi, 2020: pos.1350)

---



### O retorno: Impactos epistemológicos

Entretanto, o `output` das buscas induz a uma construção metodológica e epistemológica informada e em grande medida determinada por esse mesmo modelo de resultado.

- Em qualquer das opções de busca (*Período*, *Periódico*, *Local*), os resultados são apresentados de forma fragmentada e individualizada -  principalmente quando da busca em algum periódico que contenha apenas um *acervo*, pois o resultado retornado é a página com a primeira ocorrência e o acesso se dá de ocorrência em ocorrência sem uma percepção estruturada da distribuição das mesmas no tempo.

[PRINT DA HDB – RESULTADO DE PERIÓDICO COM ACERVO ÚNICO]

- Em periódicos que possuem vários acervos, uma lista com os *acervos* que contém ocorrências da busca é retornada, classificada através do número de ocorrências decrescentes.

[PRINT DA HDB – RESULTADO DE PERIÓDICO COM LISTA DE ACERVOS]

- Heurística de "proximidade virtual": o **potencial de encontrar fontes on-line e de selecioná-las através de uma percepção de "proximidade", possibilitada por tecnologias de organização, busca e recuperação (Solberg, 2012).** 

- Esse tipo de retorno de busca acaba limitando a possibilidade de explorar digitalmente a fundo um `database`tão monumental. Ao mesmo tempo, e consequentemente, favorece uma emulação de métodos e técnicas de pesquisa analógica, ao invés do desenvolvimento de métodos digitais mais condizentes com o tipo de dados e fontes disponíveis. 

---

<br>

### Codificando como um historiador

> Digital research methods create new and at times more stringent demands on accuracy, methodological thinkering, self-organization and colaboration than traditional historical research. (Paju, Oiva, Fridlunf, 2020, pos. 543)

---

Buscando contribuir na elaboração de caminhos heurísticos digitalmente críticos e conscientes, iremos apresentar e analisar um script de raspagem de dados criado a partir dos interesses específicos da pesquisa de um historiador utilizando a HDB.

O objetivo do programa é auxiliar à pesquisa na HDB em seus aspectos técnicos, metodológico e heurísticos ao mesmo tempo que potencializar o tratamento e análise das fontes digitalizadas, e garantir a transparência metodológica no momento da escrita e apresentação dos resultados.

---

<br>

#### Apresentação dos elementos técnicos

<div align="center">
   <p>
      <img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/noun_python.png" alt="python" style="zoom:30%;" /></p>
</div>




##### Web scraping + Python

##### BeautifulSoup

##### Selenium

##### Pandas

---

<br>

#### Apresentação do código:

##### Estrutura Geral:

Através do Selenium, o raspador acessa a página específica de um determinado jornal (a partir de uma lista com os números que identificam cada jornal, chamado `bib` ). Em seguida itera em cada acervo do jornal, realizando a busca com o termo específico, acessando cada resultado e encontrando e acumulando os dados referentes a cada ocorrência.

---

##### Organização dos diretórios

O programa cria um diretório `HDB>'nome-da-busca'>'YYYY-MM-DD'`. No interior desse diretório, serão criados três diretórios com resultados (cujos nomes de arquivos levam a data e hora de sua criação): 1) `ARQUIVOS_IMG`; 2) `CSV`; 3) `RELATÓRIOS`.

<img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/2021-04-13_00-48_pastas1.png" style="zoom:65%;" />

---

##### O CSV

As seguintes variáveis são armazenadas para cada ocorrência e inseridas em um `Dataframe`em `pandas`: Termo da busca, Data da Busca, Acervo, Ano, Edição, Página, Nome do arquivo, Link. Esse `DataFrame`é salvo como arquivo csv:

<img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/2021-04-13_00-36_csv1.png" alt="csv" style="zoom:150%;" />

---

:warning: **Download das Imagens**

As imagens em baixa resolução (por enquanto) são salvas e armazenas na pasta `ARQUIVOS_IMG` .

---

##### Os Relatórios de busca

Por fim são criados relatórios de pesquisa para cada acervo e salvos na pasta `RELATÓRIOS`.  Cada relatório possui os seguintes dados:

```
-Raspagem da HDB- 
Data e hora da busca: AAAA-MM-DD_HH-MM-SS
Termo da busca: ;
Jornal e Período: ;
Total de ocorrências: ;
Link da lista de resultados: http://memoria.bn.br/docreader/DocReader.aspx?bib=030015_02&Pesq=[busca]
```

Exemplo:

<img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/relatorio.png" alt="relatório" style="zoom:80%;" />

---

<br>

#### Análise dos resultados

<img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/noun_data search_1509987.png" style="zoom:30%;" />

##### Busca 1: "Germano Lopes da Silva"

Jornais selecionados para pesquisa (a busca acontecerá em todos os acervos de cada um deles):

- Brasil Açucareiro: Revista Quinzenal dirigida pela Comissão de Defeza da Producção do Assucar (RJ)
- Jornal do Brasil (RJ)
- O Paiz (RJ)
- Almanak Laemmert : Administrativo, Mercantil e Industrial (RJ)
- Diario Carioca (RJ)
- Gazeta de Noticias (RJ)
- O Imparcial : Diario Illustrado do Rio de Janeiro (RJ)
- O Seculo (RJ)
- Jornal do Commercio (RJ)
- A Noticia (RJ)
- Correio da Manhã (RJ)
- O Fluminense (RJ)
- Jornal dos Sports (RJ)
- A Rua : Semanario Illustrado (RJ)
- A Noite (RJ)
- Correio Official : In Medio Posita Virtus (RJ)
- O Radical (RJ)

**Foram retornadas 44 ocorrências em 17 jornais, processadas e finalizadas em 22 minutos.**

**OBS:** Esse tempo mais longo se deve em função do download das imagens de cada página com ocorrência.

Esse volume de dados é baixo e seria possível trabalhar manualmente (mas seria prudente?). Mas e se trabalhássemos com milhares de ocorrências?

---

<br>

##### Busca 2: "Monteiro Lopes"

Jornais selecionados para pesquisa (a busca acontecerá em todos os acervos de cada um deles):

- Jornal do Brasil (RJ)
- Gazeta de Notícias (RJ)
- Gazeta da Tarde (RJ)
- Jornal do Commercio (RJ)
- A Imprensa (RJ)
- O Paiz (RJ)
- Correio da Manhã (RJ)
- Revista da Semana (RJ)
- Fon Fon : Semanario Alegre, Politico, Critico e Espusiante (RJ)
- O Malho (RJ) - 1902
- O Seculo (RJ)
- A Epoca (RJ)
- Jornal do Commercio Edição da Tarde (RJ)

---

<br>

**5154 ocorrências em 13 jornais.**

![](/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/2021-04-13_01-02_csv2.png)

<br>

---

- O cálculo da média de tempo (em segundos) por ocorrência foi de **9,7 segundo**, numa internet com uma conexão de 50MB (sem o download de imagens).

- Manualmente, cada ocorrência gastou em média **um minuto para salvar todos os dados que o *script* faz** (ver vídeo). 
- Numa média de 1 minuto, para salvar todas as informações de cinco mil ocorrências seria preciso em torno de **85h de trabalho. Com o *script*, levou 14 h.**



##### Seria apenas um acelerador?

- A ferramenta garante a **coleta e organização dos dados de forma padronizada, atendendo os interesses específicos do pesquisador, possibilita a visualização desses dados também de forma organizada, torna possível retomar cada ocorrência no momento necessário ; e estabelece o registro dos caminhos da pesquisa, garantindo o rigor e transparência metodológica do trabalho.**

- Possibilita **visualização temporal, perceber volume de ocorrências em períodos específicos; localização no espaço (dependendo do conjunto de jornais pesquisados).**

---



## Conclusões

- A construção do código demanda do pesquisador um aprofundamento técnico e heurístico em relação à ferramenta de busca e ao próprio acervo que pretende buscar.
- Ou seja, precisa compreender a estrutura da ferramenta (HTML/JS/CSS) e os padrões de organização, categorização e acesso elaborados em parte por uma equipe de programadores em parte por arquivistas/bibliotecários.
- Portanto, as possibilidades de coleta e organização dos dados dependem da construção do problema e interesses de pesquisa do investigador em constante diálogo com aspectos tecnológicos e arquivísticos. Nesse sentido é improdutivo separar técnica de teoria, método de epistemologia.
- Perigo da distância entre o/a historiador/a e a elaboração das ferramentas de pesquisa e os dados que são disponibilizados;
- Importância de engajamento crítico com as ferramentas que usa;
- Literacia digital, pensar algoritmicamente.
- Desenvolver práticas de heurística digital que sejam coerentes tanto com as caracetísticas da ferramentas que usa e das fontes que vai trabalhar quanto com as reflexões teóricas básicas do ofício do/a historiador/a

---

<br>

<div align="center">
    <h4>  
    Muito obrigado pela atenção e desejo vacinação, lockdown e auxílio emergencial contra a pandemia e contra todo negacionismo e fascismo que ameaça destruir (ainda mais) esse país.
    </h4>
    <br>
    <img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/noun_injection_3862390.png" style="zoom:30%;" /> <img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/noun_lockdown_3645791.png" style="zoom:30%;" /> <img src="/home/ebn/pCloudDrive/ACADEMIA/HISTÓRIA DIGITAL/HDRio2020/Eric-Brasil_dados_HDRio/docs/assests/noun_donation_1677470.png" style="zoom:30%;" /></div>

---

## Contatos:

[Lattes](http://lattes.cnpq.br/6853705640900524) - [Orcid](https://orcid.org/0000-0001-5067-8475) - [Site](https://ericbrasiln.github.io/) - [ResearchGate](https://www.researchgate.net/profile/Eric_Brasil) - [Academia.edu](https://unilab.academia.edu/EricBrasil) - [GitHub](https://github.com/ericbrasiln/) - [Twitter](https://twitter.com/ericbrasiln) - [YouTube]()

e-mail: ericbrasiln@protonmail.com

---