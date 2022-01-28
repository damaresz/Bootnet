# Bootnet
Busca em site
Em###
# Instalar e importar a biblioteca Scrapy
pip instalar scrapy

# Criar uma pasta para o projeto 
mkdir certidão-scraper

# Navegue até o novo diretório que você acabou de criar:
cd certidao-scraper

# Em seguida, crie um novo arquivo Python para o nosso scraper chamado cert.scraper
# Você pode criar este arquivo no terminal com o comando touch.
touche cert.scraper

# criaremos uma classe Python que é uma subclasse de scrapy.Spider, uma classe básica de spider fornecida pelo Scrapy. Esta classe terá dois atributos obrigatórios:

name - apenas um nome para o spider.
start_urls - uma lista de URLs a partir da qual você começa a fazer crawling. Começaremos com uma URL.
Abra o arquivo cert.scrapy em seu editor de texto e adicione este código para criar o spider básico:

# código

import scrapy


class BrickSetSpider(scrapy.Spider):
    name = "certidao_spider"
    start_urls = ['http://...']
    
    # Interface de comando de linha
    scrapy runspider cert.scraper
    
    # Dentro do log gerado pela execução do spider é possível confirmar a as informações coletadas.
    # Após teste inicial feito sera lancados as leituras dos dados web
    # pode colocar quantos links quiser, já com os "dados preenchidos' e com todos os dados necessário, para isso 
    
    # class NoticiasItem(scrapy.Item):
    title = scrapy.Field()
    author = scrapy.Field()
    text = scrapy.Field()
    link = scrapy.Field()
    # 
