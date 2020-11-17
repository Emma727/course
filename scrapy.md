### start project

##### code:

scrapy startproject projectname

scrapy shell "web_url"  (to try extract information)


### select css
response.css('title::text').ext

### select Xpath

response.xpath("//span[@class='text']/text()").extract()



### output files
scrapy crawl quotes -o items.json




