# Classificação de Câncer de Mama por Imagens - CBIS-DDSM

Sistema de Deep Learning para classificação de mamografias em benignas ou malignas, desenvolvido como parte do Tech Challenge da FIAP. O projeto utiliza o dataset CBIS-DDSM (Curated Breast Imaging Subset of DDSM) e implementa uma Rede Neural Convolucional (CNN) para análise direta de imagens médicas.

## Sobre o Projeto

Este projeto foi desenvolvido para atender aos requisitos do Tech Challenge, focando na aplicação de técnicas de Deep Learning para classificação de câncer de mama usando imagens de mamografia. O sistema utiliza uma CNN para processar imagens diretamente, aprendendo padrões automaticamente sem necessidade de extração manual de features.

## Dataset

O dataset utilizado é o **CBIS-DDSM (Curated Breast Imaging Subset of DDSM)**, disponível no Kaggle e amplamente utilizado em pesquisas sobre diagnóstico de câncer de mama por imagens.

### Características do Dataset

- **Total de amostras**: Mais de 3.000 mamografias
- **Formato**: Imagens JPEG (originalmente DICOM)
- **Resolução**: Redimensionadas para 384x384 pixels
- **Distribuição das classes**:
  - Benigno: ~64%
  - Maligno: ~36%
- **Tipos de lesões**: Calcificações e massas, cada uma classificada como benigna ou maligna

### Estrutura dos Dados

- Imagens organizadas em `dataset/jpeg/`
- Metadados em CSVs: `training_dataset.csv` e `test_dataset.csv`
- Mapeamento de rótulos:
  - 1 e 3 → Maligno
  - 2 e 4 → Benigno

## Estrutura do Projeto

```
breast-cancer-classification/
├── dataset/
│   ├── csv/
│   │   ├── training_dataset.csv
│   │   └── test_dataset.csv
│   └── jpeg/
│       └── [estrutura de diretórios com imagens]
├── main.ipynb                        # Notebook principal com toda a análise
├── requirements.txt                  # Dependências do projeto
└── README.md                         # Este arquivo
```

## Instalação e Configuração

### Pré-requisitos

- Python 3.7 ou superior
- pip (gerenciador de pacotes Python)

### Instalação das Dependências

1. Clone o repositório:
```bash
git clone <url-do-repositorio>
cd breast-cancer-classification
```

2. Instale as dependências:
```bash
pip install -r requirements.txt
```

### Execução

Abra o notebook Jupyter:
```bash
jupyter notebook main.ipynb
```

Ou use JupyterLab:
```bash
jupyter lab main.ipynb
```

## Licença

Este projeto está sob a licença especificada no arquivo LICENSE (se aplicável).

## Autor

Desenvolvido como parte do Tech Challenge da FIAP - Especialização em Inteligência Artificial e Machine Learning.

## Contribuições

Este é um projeto acadêmico desenvolvido para o Tech Challenge. Sugestões e melhorias são bem-vindas através de issues ou pull requests.

