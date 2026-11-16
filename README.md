# Projeto M2.2 - Filtragem na Frequência, Morfologia e Segmentação

## Descrição
Este repositório contém a implementação do **Projeto M2.2 – Filtragem na Frequência, Morfologia e Segmentação**, desenvolvido para a disciplina de Processamento de Imagens.

O trabalho foi desenvolvido em `Python` utilizando o `Google Colab` e aborda técnicas de processamento digital de imagens divididas em duas partes. A primeira explora a filtragem no domínio da frequência e a comparação entre os algoritmos de segmentação Watershed e SLIC em imagens com ruído Gaussiano. A segunda aborda a segmentação morfológica de imagens de microscopia celular, utilizando limiarização de Otsu, operações morfológicas, preenchimento de buracos (*gap-filling*) e contagem automatizada de células.

## Disciplina:
Processamento de Imagens 

## Acadêmicas:
- Beatriz Pimentel Bagesteiro Alves
- Maria Eduarda Santos
- Yasmin Tarnovski Faccin

## Conteúdo
- **Parte I – Filtragem na Frequência e Segmentação com Watershed e SLIC:**
  - Seleção e caracterização da imagem;
  - Inserção de ruído Gaussiano;
  - Aplicação de filtros no domínio da frequência;
  - Implementação e comparação dos filtros Gaussiano e Butterworth;
  - Visualização dos espectros de frequência antes e depois da filtragem;
  - Aplicação da transformada inversa para retornar ao domínio espacial;
  - Segmentação utilizando os algoritmos Watershed e SLIC;
  - Comparação das regiões segmentadas e dos contornos obtidos;
  - Avaliação da qualidade utilizando as métricas PSNR e SSIM.

- **Parte II – Segmentação Morfológica e Gap-Filling para Contagem de Células:**
  - Leitura das imagens de microscopia celular;
  - Aplicação de limiarização automática pelo método de Otsu;
  - Análise de falhas na segmentação inicial, como buracos internos, contornos fragmentados e ruídos;
  - Implementação de operações morfológicas com elementos estruturantes circulares;
  - Aplicação de fechamento morfológico;
  - Implementação do preenchimento de buracos (*gap-filling*), incluindo o tratamento de células nas bordas da imagem por espelhamento;
  - Aplicação de abertura morfológica para remoção de pequenas partículas;
  - Implementação de algoritmo próprio para contagem automatizada de células;
  - Comparação da contagem antes e depois do pós-processamento morfológico;
  - Visualização das imagens originais, após limiarização, após morfologia e com os rótulos coloridos de cada célula.

## Tecnologias utilizadas
- Python
- Google Colab
- OpenCV
- NumPy
- Matplotlib
- scikit-image
 
## Arquivo

O arquivo `.ipynb` está disponível neste repositório. Como o notebook possui um tamanho grande, ele pode não ser exibido diretamente pelo GitHub.

Para visualizar e executar o trabalho, é necessário **baixar o arquivo `.ipynb` e abri-lo no Google Colab**.

- `projeto_m2_2_filtragem_na_frequencia_morfologia_e_segmentacao.ipynb` - Notebook com as implementações, testes, comparações e resultados das duas partes do trabalho.

## Imagens utilizadas

O trabalho utiliza imagens de diferentes bases de dados, conforme as duas partes do projeto:

- **Parte I:** imagem selecionada do **VOC2012**, utilizada nos testes de filtragem na frequência e segmentação com Watershed e SLIC.
- **Parte II:** imagens de microscopia celular do dataset **BBBC006**, utilizadas nos testes de limiarização, operações morfológicas e contagem automatizada de células.
