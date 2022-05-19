# Apify Scrapy Executor
Support module for [Apify Scrapy Migrator](https://pypi.org/project/apify-scrapy-migrator/). Runs migrated Scrapy 
project and uploads result to Apify default dataset.

## Usage
Since [`apify-client`](https://pypi.org/project/apify-client/) does not fully support local runs yet, migrated 
Scrapy projects work best on Apify Cloud. Apify Scrapy Migrator is recommended to be used with Apify Scrapy Migrator on
Apify Cloud.

But for people who want to earn their results, here is a small example.

```python
# import SpiderExecutor class
from apify_scrapy_executor import SpiderExecutor
# create instance of the Spider executor class with scrapy class as an argument
spider_executor = SpiderExecutor(scrapy_class)
# run the scrapy project with dataset_id argument to save the result and args_dict for scrapy input
spider_executor.run(dataset_id=apify_dataset, args_dict=actor_input)
```
