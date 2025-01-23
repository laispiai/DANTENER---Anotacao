# DANTENER---Anotacao
**O objetivo desse repositório é abrigar o processo da segunda anotação de Entidades Nomeadas no [DANTEStocks](https://sol.sbc.org.br/index.php/stil/article/view/17813/17647)**.
Esse é um corpus de material textual compilado do Twitter, atualmente X. As postagens foram coletadas automaticamente em 2014 com base nos tickers (código das ações) negociados pelo índice IBOVESPA. Este é o primeiro corpus em português de conteúdo gerado por usuários (user-generated content - UGC) com anotação seguindo o modelo Universal Dependencies (UD). A versão utilizada para esta anotação corresponde à disponibilizada em 15/12/2022. Esta é a segunda anotação de Entidades Nomeadas (EN) realizada no corpus DANTE, com o objetivo de expandir a anotação realizada por [Zerbinati et al. (2024)](https://aclanthology.org/2024.propor-1.28/). Esse trabalho faz parte da dissertação de mestrado em linguística "Caracterização de entidades nomeadas em um corpus de tweets: contribuição para o processamento automático do português" da aluna Laís Piai. /

 Este trabalho foi apoiado pelo Ministério da Ciência, Tecnologia e Inovações, com recursos da Lei N. 8.248, de 23 de outubro de 1991, no âmbito do PPI-Softex, coordenado pela Softex e publicado como Residência 
 em TIC 13, DOU 01245.010222/2022-44.


# Resumo da estrutura de diretórios e arquivos:
* **_Corpus_**
  * Última versão do _corpus_ anotado.
  * A versão utilizada é de 15/12/2022 no formato conllu. Contém 4.048 tweets e 84.396 tokens.
    
* **Decisões da anotação**
  * Arquivo com as decisões de anotação tomadas para casos de dúvida.

* **Tagset**
  * Conjunto de etiquetas possíveis, conforme a marcação BIOES e a taxonomia utilizada baseada no Segundo HAREM [(Mota; Santos, 2008)](https://www.linguateca.pt/LivroSegundoHAREM/)

* **Pasta com as regras usadas para anotar automaticamente entidades no corpus.**
  * As regras baseadas em _regex_ foram executadas no ambiente de anotação [Interrogatório](https://github.com/alvelvis/Interrogat-rio)
* **Instâncias anotadas**
  * Contém pasta com as instâncias anotadas. Estão separados por categorias em arquivos JSON.
  * Arquivo JSON com as instâncias anotadas em mais de uma categoria.



