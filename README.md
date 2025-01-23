# DANTENER---Anotacao
**O objetivo desse repositório é abrigar o processo da segunda anotação de Entidades Nomeadas no DANTEStocks**.
Esse é um corpus de material textual compilado do Twitter, agora X. As postagens foram coletadas automaticamente em 2014 com base nos tickers (código das ações) negociados pelo índice IBOVESPA. Este é o primeiro corpus em português de conteúdo gerado por usuários (em inglês, user-generated content - UGC) com anotação Universal Dependencies (UD). O corpus utilizado nesta anotação corresponde a versão do DANTEStocks disponibilizada em **15/12/2022**. Está é a segunda anotação de EN no Dante e visa estabeler um padrão ouro, além de expandir a primeira anotação. Esse trabalho faz parte da dissertação de mestrado em linguística "Caracterização de entidades nomeadas em um corpus de tweets: contribuição para o processamento automático do português" da aluna Laís Piai. 

# Resumo da estrutura de diretórios e arquivos:
* **_Corpus_**
  * Última versão do _corpus_ anotado.
  * A versão utilizada é de 15/12/2022. Contém 4.048 tweets e 84.396 tokens.
    
* **Decisões da anotação**
  * Arquivo com as decisões de anotação tomadas para casos de dúvida.

* **Tagset**
  * Conjunto de etiquetas possíveis, conforme a anotação BIOES e a taxonomia utilizada.

* **Pasta com as regras usadas para anotar automaticamente entidades no corpus.**
  * As regras baseadas em _regex_ foram executadas no ambiente de anotação Interrogatório (https://github.com/alvelvis/Interrogat-rio)
* **Instâncias anotadas**
  * Contém pasta com as instâncias anotadas. Estão separados por categorias em arquivos JSON.
  * Arquivo JSON com as instâncias anotadas em mais de uma categoria.
  


