# Alocação dinâmica de recursos para formação de fatias de rede em ambientes de demanda elástica

Repositório da monografia de **Francisco das Chagas Duarte Rodrigues**, do Curso de Ciências da Computação da **Universidade Estadual Vale do Acaraú (UVA)**, sob orientação de **Walisson Ferreira Pereira**. Sobral, 2026.

## Sobre o trabalho

As variações na demanda dos usuários da Internet motivam a busca por formas mais flexíveis de gerenciar os recursos dos provedores de serviços de Internet (ISPs). Nesse contexto, o fatiamento de rede (*network slicing*) permite particionar recursos e funções em fatias virtuais destinadas aos requisitos de diferentes usuários e aplicações, visando melhorar a qualidade de serviço (QoS).

O trabalho aborda a alocação dinâmica de recursos para a formação dessas fatias em ambientes de demanda elástica. Apresenta uma visão introdutória do conceito de fatiamento de rede e das abordagens que possibilitaram sua evolução, seguida da apresentação e comparação de algoritmos de fatiamento. A comparação busca caracterizar as abordagens e identificar os cenários em que cada algoritmo apresenta melhor desempenho.

**Palavras-chave:** fatiamento de rede; demanda elástica; alocação de recursos; algoritmos de fatiamento; virtualização de redes; qualidade de serviço.

> Esta apresentação se baseia no conteúdo temático do abstract em `capitulos/resumole.tex` e nos dados de `monografia.tex`. Os arquivos de resumo ainda contêm trechos de exemplo (Lorem Ipsum), que precisam ser substituídos na monografia.

## Estrutura do repositório

| Caminho | Conteúdo |
| --- | --- |
| `monografia.tex` | Documento principal, dados acadêmicos e organização da monografia. |
| `capitulos/` | Capítulos e elementos pré-textuais, incluindo resumo e abstract. |
| `referencias.bib` | Referências bibliográficas em formato BibTeX. |
| `figuras/` | Imagens utilizadas no documento. |
| `apendices/` | Arquivos de apêndices. |
| `anexos/` | Arquivos de anexos. |
| `uva.sty` | Estilo local de formatação institucional, utilizado com a classe `abntex2`. |
| `pgf-pie.sty` | Pacote local para gráficos de setores. |

## Compilação

É necessária uma distribuição LaTeX com `pdfLaTeX`, `BibTeX`, `MakeIndex`, a classe `abntex2` e os pacotes carregados por `uva.sty`.

Na raiz do repositório, execute:

```sh
pdflatex monografia.tex
bibtex monografia
makeindex monografia.idx
pdflatex monografia.tex
pdflatex monografia.tex
```

O documento gerado será `monografia.pdf`. O `.gitignore` exclui esse PDF e os arquivos auxiliares de compilação, preservando os PDFs utilizados como fontes em anexos e apêndices.
