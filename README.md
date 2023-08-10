# Newspaper Article scraping,language conversion and summarization.

A simple implementation of scraping the newspaper article,  then converting the langauge into the english lanugage using the helsinki hugging face model.Then summarizing the converted data in short for easy reading and understanding of any language newspaper.


## Requirements
```shell
pip install -r requirements.txt

```shell
python -m nltk.downloader punkt

If the punkt error comes even after running commands :
pip install -r requirements.txt

Then run command:
```shell
python try.py

## commands to run: 
To run the file locally: 
```shell
python main.py

To run the application using the Fastapi: 
```shell
uvicorn api:app --reload 

## Files
* scrap.py: This file include the scraping of the article data of newspaper including Title,Text,Summary,Keywords,URL and savinf in the scrap_newspaper folder. 
* convert.py: This file will convert the language other than english into the english language nad save the file in the csv format in converted_data folder.
* summarize.py: This file will summarize all the articles in short and store it into the new csv file and store it into the summarize_data folder.
* main.py:running this file will initiate the application in the terminal locally
* api.py: To start the application using the uvicorn Fastapi.



