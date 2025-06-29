# DANTENER — Anotação de Entidades Nomeadas

**O objetivo deste repositório é abrigar a segunda anotação de Entidades Nomeadas no [DANTEStocks](https://sol.sbc.org.br/index.php/stil/article/view/17813/17647)**, expandindo aquela realizada por [Zerbinati et al. (2024)](https://aclanthology.org/2024.propor-1.28/), disponível também no [Repositório ner_financial_tweets_portuguese](https://github.com/mzerbinatti/ner_financial_tweets_portuguese).

Este trabalho é resultado da dissertação *"Anotação de Corpus: Caracterização de Entidades Nomeadas em Tweets do Mercado Financeiro"*, desenvolvida por Laís Piai, aluna do Programa de Pós-Graduação em Linguística da UFSCar.

O DANTEStocks é um _corpus_ de material textual compilado a partir do Twitter (atualmente X). As postagens foram coletadas automaticamente em 2014 com base nos *tickers* (códigos das ações) negociadas pelo índice IBOVESPA naquele ano.

Este é o primeiro _corpus_ em português de conteúdo gerado por usuários (*user-generated content* – UGC) com anotação seguindo o modelo Universal Dependencies (UD).

A versão utilizada nesta anotação corresponde à versão 1.0, disponibilizada em 15/12/2022, que contava apenas com anotação POS à época. Especificamente, possui **4.048 tweets** e um total de **84.396 tokens**. Outras versões estão descritas e disponíveis na página do projeto [Porttinari 2.0](https://sites.google.com/icmc.usp.br/poetisa/porttinari-2-0).

---

## 📁 Estrutura de Diretórios e Arquivos

### **Corpora**
- Contém:
  - A versão 1.0 do DANTEStocks.
  - A última versão do *corpus* anotada (a anotação está codificada na quinta coluna – XPOS).

### **Guia de Anotação**
- Manual de anotação de entidade nomeada (EN):
  - **"Guia de Anotação de Entidades Nomeadas em Tweets do Mercado Financeiro: Adaptação da Taxonomia Hierárquica do Segundo HAREM"**

### **Tagset**
- Conjunto de etiquetas possíveis conforme a marcação BIOES e a taxonomia baseada no Segundo HAREM [(Mota & Santos, 2008)](https://www.linguateca.pt/LivroSegundoHAREM/).
- Abrange 10 categorias:
  - **ABSTRAÇÃO, ACONTECIMENTO, COISA, LOCAL, OBRA, ORGANIZAÇÃO, PESSOA, TEMPO, VALOR e OUTRO**
- Inclui também 4 tipos específicos:
  - `certificado`, `indicador`, `ticker` (na categoria COISA) e `usuário` (na categoria PESSOA).

### **Regras**
- Pasta contendo as regras baseadas em expressões regulares (regex) utilizadas para a anotação automática das entidades.
- As regras foram aplicadas por meio do ambiente de anotação [Interrogatório](https://github.com/alvelvis/Interrogat-rio).

### **Entidades Anotadas**
- Contém:
  - Arquivo `.json` com expressões anotadas em mais de uma categoria.
  - Arquivo `.xlsx` com a lista de entidades **unitárias** (compostas por um único token).
  - Arquivo `.xlsx` com a lista de entidades **multipalavra** (compostas por mais de um token).
  - **Arquivo `.json` com Entidades e POS Tags**:
    - A estrutura do arquivo consiste em uma lista de objetos, onde cada objeto representa um tweet e contém:
      - `doc_id`: identificador do tweet.
      - `doc_text`: texto completo do tweet.
      - `entities`: lista de entidades com texto, categoria, tipo e *offsets* (posição no texto).
      - `pos_tags`: lista de classes gramaticais para cada token, incluindo *offsets*.

---

## Financiamento

Este trabalho foi apoiado pelo Ministério da Ciência, Tecnologia e Inovações, com recursos da Lei nº 8.248, de 23 de outubro de 1991, no âmbito do **PPI-Softex**, coordenado pela **Softex**, e publicado como **Residência em TIC 13**, DOU 01245.010222/2022-44.
