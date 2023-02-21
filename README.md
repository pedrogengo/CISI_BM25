# CISI BM25

**Author:** Pedro Gabriel Gengo Lourenço

## 1. Descrição

## 2. How ChatGPT was used?

I used ChatGPT to provide some guidelines about how to start the code for preprocess CISI dataset and for create the index that will be used in BM25 algorithm. To make sure that ChatGPT will understand that I was talking about the CISI dataset in the context of information retrieval I started asking about BM25 and information retrieval to create some context in ChatGPT.

After that, I asked to it writes a python code to download and open the CISI files (cisi.all, cisi.qry and cisi.rel). The code returned by ChatGPT was based in regex to parse the documents, but the regex provided didn't cover some edge cases. One example is a regex that started like `W.\n`, but in the texts we have some person last names that finished with `W.` and the regex provided by ChatGPT matched with it, which doesn't make sense. So, I changed some parts of the answer provided by ChatGPT and apply some sanity checks just to make sure that I was parsing the right number of documents at least.

Then, I asked to ChatGPT to make a code 

## 3. Repository structure
```
.
└── CISI_BM25/
    ├── notebooks/
    │   ├── Developing_BM25.ipynb: walkthrough about how BM25 and implementation
    │   └── Downloading_and_Processing_CISI.ipynb: walkthrough about how to download and parse CISI dataset
    ├── README.md
    └── LICENSE
```

## 4. How to run

To be easy, I decided to keep everything in one colab (if you want further explanation about each step, you can go to the notebooks inside the `notebooks` folder). You just need to execute all cells in the straight order and check the results at the end

## Resultados

## Conclusões

## Melhorias
