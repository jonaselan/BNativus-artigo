# BNativus-artigo

Além do meu TCC versionado, nesse repositório está um pequeno tutorial de como usar o LaTeX baseado em um exemplo pre pronto disponibilizado pelo site da [DIATINF](http://diatinf.ifrn.edu.br/doku.php).

## LaTeX [?](https://pt.wikipedia.org/wiki/LaTeX)

LaTeX é um conjunto de macros para o programa de diagramação de textos TeX, utilizado amplamente na produção de textos matemáticos e científicos, devido a sua alta qualidade tipográfico. Entretanto, também é utilizado para produção de cartas pessoais, artigos e livros sobre assuntos diversos. O sistema LaTeX fornece ao usuário um conjunto de comandos de alto nível, facilitando dessa forma sua utilização por iniciantes. Possui abstrações para lidar com bibliografias, citações, formatos de páginas, referência cruzada e tudo mais que não seja relacionado ao conteúdo do documento em si.

## Motivação

Quando decidi usar o LaTeX para montar toda a estrutura da parte escrita do meu TCC, tive algumas dificuldades, apesar de ser uma línguagem de marcação, como a que estou usando para escrever esse texto. Pensei que provavelmente outros alunos do curso irão passar pelos mesmos problemas, então decidi montar um pequeno tutorial, para poupar o tempo que gastei. Espero que seja útil.

## CRIAR UM NOVO PROJETO

1. [Baixe](http://diatinf.ifrn.edu.br/lib/exe/fetch.php?media=cursos:superiores:tads:praticas:tcc:modelo_tcc_latex-placido.zip) o modelo encontrado no site da DIATINF

2. Vá até algum editor de LaTeX, como o overleaf ou Shared latex

3. Crie um novo projeto e faça o upload do zip baixado no item 1

## USANDO

Os trechos de códigos a seguir são voltados para o modelo que o [Prof. Plácido](https://github.com/placidoneto) criou, que já inclui algumas bibliotecas que auxiliam na construção do texto. Se for iniciar um novo projeto do zero, dê um olhada neste (arquvio)[https://github.com/jonaselan/BNativus-artigo/blob/master/src/main.tex], que é aonde os arquivos e estas bibliotecas estão sendo importadas.

- Itálico: `\textit{TEXTO}`

- Negrito: `\textbf{TEXTO} `

- Sublinhado: `\underline{TEXTO}`

- Centralizar texto:
`
\begin{center}
TEXTO
\end{center}
`
- Capítulo: `\chapter{NOME}`

- Seção: `\section{NOME}`

- Subseção: ``

- Observação: `\todo[inline]{TEXTO}`

- [Lista](https://pt.wikibooks.org/wiki/Latex/Itens)
  - Normal

    ```
    \begin{itemize}
        \item ITEM1;
        \item ITEM2.
    \end{itemize}
    ```
  - Numerada

    ```
    \begin{enumerate}
       \item item1
       \item item2
     \end{enumerate}
     ```

- [Imagem](https://www.sharelatex.com/learn/Inserting_Images)

```
\begin{figure}[htb]
  	\includegraphics[scale=0.60]{src/imagens/IMAGEM.png}
  	\textsf{\caption{DESCRIÇÃO}}
  	\label{fig:FiguraTeste}
\end{figure}
```

O `htb` representa onde a imagem vai ficar alocada na página. O **h** é no centro, o **t** é de cima e o **b** para ser posicionada em baixo. Para força a posição em algum lugar, coloque **!** no início, como **[!htb]**.

- Abreviação: `\abrv[IFRN -- Instituto Federal do Rio Grande do Norte]{IFRN}`

Ao especificar em qualquer lugar do texto, já adicionado a lista de abreviações.

- Quebra da página: `\newpage`

- Referência

- Tabela: A forma mais fácil de criar tabelas é através de ferramentas online, como [essa](https://www.tablesgenerator.com/#) onde é você monta a tabela e o código latex é gerado.

- Rodapé


## Contribuição

Esse repositório foi criado para auxiliar outros alunos do curso de TADS que estão começando a ~sofrer~ escrever seus trabalhos. Se notar alguma coisa que escrevi errado ou quiser melhorar, vá em frente e faça o fork :)

1. Fork o projeto
2. Criar uma branch com as suas sugestões (git checkout -b nova-branch)
3. Commite as mudanças (git commit -am 'Sugestão')
4. Push (git push origin nova-branch)
5. Criar Pull Request (PR)

Boa escrita!
