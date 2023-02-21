# Avaliando BM25 no CISI

**Author:** Pedro Gabriel Gengo Lourenço

## 1. Descrição

Esse repositório contém todo o código desenvolvido para o processo de seleção da disciplina "Deep Learning aplicado a sistemas de buscas" ofertada no primeiro semestre de 2023 pela FEEC-Unicamp. O exercício proposto solicitou a construção de um sistema de recuperação de informação usando o algoritmo BM25 e avaliando os resultados no dataset CISI. Além disso, foi estimulado o uso do ChatGPT para auxiliar durante toda a construção da solução.

Na seção [2](#2) do presente relatório é descrito como o ChatGPT foi utilizado para a resolução do desafio proposto. Na seção [3](#3) é apresentada a estrutura do repositório, assim como uma descrição de cada um dos arquivos. Na seção [4](#4) é explicado como reproduzir o experimento e as seções [5](#5), [6](#6) e [7](#7) apresentam os resultados em relação ao dataset CISI, assim como as conclusões e possíveis melhorias.

## <a name="2"></a>2. Como o ChatGPT foi utilizado?

I used ChatGPT to provide some guidelines about how to start the code for preprocess CISI dataset and for create the index that will be used in BM25 algorithm. To make sure that ChatGPT will understand that I was talking about the CISI dataset in the context of information retrieval I started asking about BM25 and information retrieval to create some context in ChatGPT.

After that, I asked to it writes a python code to download and open the CISI files (cisi.all, cisi.qry and cisi.rel). The code returned by ChatGPT was based in regex to parse the documents, but the regex provided didn't cover some edge cases. One example is a regex that started like `W.\n`, but in the texts we have some person last names that finished with `W.` and the regex provided by ChatGPT matched with it, which doesn't make sense. So, I changed some parts of the answer provided by ChatGPT and apply some sanity checks just to make sure that I was parsing the right number of documents at least.

Then, I asked to ChatGPT to make a code 

## <a name="3"></a>3. Estrutura do repositório
```
.
└── CISI_BM25/
    ├── notebooks/
    │   ├── Developing_BM25.ipynb: walkthrough about how BM25 and implementation
    │   └── Downloading_and_Processing_CISI.ipynb: walkthrough about how to download and parse CISI dataset
    ├── README.md
    └── LICENSE
```

## <a name="4"></a>4. Como reproduzir o experimento?

To be easy, I decided to keep everything in one colab (if you want further explanation about each step, you can go to the notebooks inside the `notebooks` folder). You just need to execute all cells in the straight order and check the results at the end

## <a name="5"></a>5. Resultados

## <a name="6"></a>6. Conclusões

## <a name="7"></a>7. Melhorias
