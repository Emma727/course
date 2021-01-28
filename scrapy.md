* 目录
    1. code
        1. start project
        2. select css
        3. select Xpath
        4. output files
    2. 注意事项



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

## 注意事项

1. 写翻页爬虫的时候要注意判断当前页面是否有内容。很可能是第一页就没有内容的。




