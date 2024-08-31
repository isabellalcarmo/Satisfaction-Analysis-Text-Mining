<h1 align="center">
Análise de Satisfação de Serviços e Produtos Brasileiros em
Plataformas Eletrônicas: Uma Abordagem de Mineração de Texto
</h1>

<div align="center">
Isabella Lopes Carmo dos Santos
</div>

## ✒️ Descrição
Este repositório contém o código e os materiais relacionados ao desenvolvimento de uma metodologia para compreender opiniões e sentimentos dos consumidores após a prestação de serviços e a venda de produtos em plataformas eletrônicas brasileiras. Utilizando técnicas de mineração de texto, o estudo concentra-se em três principais áreas:

- Modelagem de Tópicos: Identificação de temas recorrentes nos comentários dos consumidores.
- Análise de Sentimentos: Avaliação das emoções expressas nas avaliações.
- Extração de Entidades Nomeadas: Identificação de entidades relevantes mencionadas pelos consumidores.

A metodologia foi aplicada a dados públicos de avaliações de diversos setores, com o objetivo de auxiliar empresas e comerciantes a melhorar seus produtos, serviços e atendimento ao cliente.

## 🗒️ Conjuntos de Dados
Os conjuntos de dados utilizados incluem avaliações obtidas de fontes públicas disponíveis online. O único conjunto de dados que não foi obtido online foi o do restaurante Guacamole no TripAdvisor, que foi coletado através de técnicas de web scraping diretamente do site, respeitando os termos de uso e políticas de privacidade da plataforma.

- Olist: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce
- Buscapé: https://www.kaggle.com/datasets/fredericods/ptbr-sentiment-analysis-datasets
- B2W Digital: https://github.com/americanas-tech/b2w-reviews01
- Hotéis Brasileiros: https://data.mendeley.com/datasets/2w3kvrg97m/1

## 💻 Aplicação do Método
O método foi aplicado utilizando técnicas e modelos baseados no BERT, como o [BERTopic](https://github.com/MaartenGr/BERTopic) para a modelagem de tópicos e [BERTimbau](https://neuralmind.ai/bert/) para a análise de sentimentos onde, para esse último, foi utilizado um [modelo treinado](https://drive.google.com/file/d/1Ek23dYUtHTxzS9nqL3V8m-Gc7no-2TTD/view?usp=sharing) através do BERTimbau usando as avaliações da Olist, da Buscapé, da B2W Digital e UTLC. O mesmo obteve uma acurácia de 78% e retorna resultados com valores de "positivo", "neutro" e "negativo". Por fim, para a extração de entidades nomeadas, foi utilizado um [modelo](https://huggingface.co/51la5/roberta-large-NER) treinado com o RoBERTa.
