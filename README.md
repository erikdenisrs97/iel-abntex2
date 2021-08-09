# O que é o iel-abntex2?

O iel-abntex2 é um projeto baseado no [abnTeX2](https://github.com/abntex/abntex2) e que foi desenvolvido com o intuito de auxiliar os alunos da IEL em seus trabalhos acadêmicos.
É importante que o aluno saiba pelo menos um pouco sobre LaTeX pois aqui ele não encontrará informações específicas sobre o funcionamento do LaTeX e/ou abnTeX2. Caso não saiba, consulte [Iniciando em LaTeX](https://github.com/abntex/abntex2/wiki/PorOndeComecar) e também veja alguns no Youtube.

> Segundo a [The LaTeX Project Public License](http://www.latex-project.org/lppl.txt) você é livre para conhecer, estudar, alterar e redistribuir o trabalho do abnTeX2.

# Como utilizar?

 1. O aluno deve fazer o Download do projeto clicando [aqui](https://github.com/erikdenisrs97/iel-abntex2/archive/refs/heads/main.zip) ou utilizar o `git clone`;
 2. É necessário definir um editor e compilador para o documento. Recomendo o uso do [Overleaf](pt.overleaf.com) porque ele funciona diretamente no browser e assim você não precisa instalar nada no seu computador;
 3. Basta fazer o upload projeto no seu editor preferido, abrir o **documento.tex** e redigir seu trabalho acadêmico. O documento possuí comentários que são auto-explicativos.
 
> Você é iniciante? [Essa página](http://www.abntex.net.br/) é desenvolvida pela equipe do abnTeX e contém muitas informações importantes.

> Na pasta manuais há um documento específico para o abnTeX2.

# Customizações Realizadas

 - Alteração da capa e folha de rosto;
 - Adicação do cabeçalho e rodapé da IEL na capa e folha de rosto;
 - Toda a fonte do documento é Helvética (Arial), tamanho 12pt;
 - Alterado o espaçamento entre parágrafos;
 - Removido a página que indica o início dos Apêndices;
 - Removido a página que indica o início dos Anexos;
 - Resumos apenas em Português e Inglês;
 - O sumário foi alterado para o formato tradicional e modificações foram realizadas.
 - Títulos dos trabalhos nas referências em negrito;
 - Contador de quantas vezes o autor foi citado no documento e respectivas páginas.

# Importante

 - O iel-abntex2 não têm vínculo com o IEL / Faculdades da Indústria;
   Não possuí nenhuma garantia e pode ser distribuido e alterado livremente para fins acadêmicos;
 - É possível que o iel-abntex2 sofra alterações ao longo do tempo,
   corrigindo possíveis falhas, implementando novas funções ou alterações no estilo.

# Dicas

## Inserindo Figuras

```latex
\begin{figure}[!htb]
	\centering
	\caption{Logo Faculdades da Indústria}
	\includegraphics[scale = 0.5]{images/Faculdade-da-Indústria-IEL-25.png}
	\fonte{\citeonline{abntex2-wiki-como-customizar}}
\end{figure}
```
## Inserindo Capitulos
```latex
\chapter{Meu Capítulo}
```
## Inserindo Seções
```latex
\section{Minha Seção}
\subsection{Minha Subseção}
\subsubsection{Minha SubSubseção}
```
## Inserindo Tabelas

```latex
\begin{table}[]
\begin{tabular}{ll}
\rowcolor[HTML]{CBCEFB} 
\multicolumn{1}{c}{\cellcolor[HTML]{CBCEFB}Estado} & Cidade         \\
Paraná                                             & Curitiba       \\
Fortaleza                                          & Ceará          \\
Minas Gerais                                       & Belo Horizonte
\end{tabular}
\end{table}
```

> Acesse o site [Table Generator](https://www.tablesgenerator.com/) para gerar tabelas com mais facilidade.

## Referenciando

As referências ficam contidas no arquivo **referencias.bib**. Nele há vários exemplos de como as referências podem ser inseridas.

Para inserir a referência no documento:

```latex
\citeonline{abntex2-wiki-como-customizar}
\cite{ibge1993}
```

## Inserindo Quadros

```latex
\begin{quadro}[htb]
\caption{\label{quadro_exemplo}Exemplo de quadro}
\begin{tabular}{|c|c|c|c|}
	\hline
	\textbf{Pessoa} & \textbf{Idade} & \textbf{Peso} & \textbf{Altura} \\ \hline
	Marcos & 26    & 68   & 178    \\ \hline
	Ivone  & 22    & 57   & 162    \\ \hline
	...    & ...   & ...  & ...    \\ \hline
	Sueli  & 40    & 65   & 153    \\ \hline
\end{tabular}
\fonte{Autor.}
\end{quadro}
```