# Análise do Catálogo do Netflix
Este é um trabalho desenvolvido para a disciplina da Estrutura de Dados II no 4º semestre em conjunto com outros alunos.  
A análise utilizou *árvore AVL* para armazenar os dados. Também foi utilizado *árvore BST*, mas apenas para verificar as *diferenças* de *performance* na operação de pesquisa entre a AVL e a BST.  
Os dados foram fornecidos pelo Professor Ivan Carlos Alcantra de Oliveira por meio de um arquivo CSV.  
Os dados estão atualizados até 2022. Ou seja, não há fimles ou séries que surgiram a partir de 2023.  
Todas análises feitas utilizam algum dos tipos de percurso em árvore: pré, pós ou em ordem.  
# Análises feitas:  
### Verificar quais programas voce pode assistir de acordo com sua idade:
Esta análise mostra quais e quantos fimles/séries o usuário pode assistir ao inserir a idade.  
É solicitado ao usuário a opção de imprimir o nome dos programas ou não, pois a lista dos filmes/séries pode ser muito grande.  
***
### Mostrar 5 melhores filmes e 5 piores filmes de um dado gênero
Esta análise mostra um ranking dos 5 melhores filmes e os 5 piores deles considerando o gênero que o usuário escreveu.  
A análise utiliza a nota do IMDB para determinar os melhores e piores filmes.  
***
### Top 5 series mais populares
Esta análise mostra quais são as 5 séries mais populares.  
A análise utiliza do valor que está presente no TMDB.  
***
### Comparar score da critica(imdb) com o score do publico(tmdb)
Esta análise faz uma comparação entre as notas da IMDB com o do TMDB.  
É apresentado a opção de comparar um filme/série em específico ou em comparar em geral.  
Ao escolher fazer a comparação com um título em específico, é pedido um ID em específico. Este ID está presente em todos os filmes/séries do arquivo CSV.  
*Adendo*: podem existir títulos com dados insuficientes para esta análise.  
***
### Quantidade de filmes em cada categoria e suas respectivas porcentagens diante o total
Esta análise faz o cálculo da quantidade de filmes em cada categoria e a respectiva porcentagem diante do total.   
É apresentado cada gênero, a quantidade bruta e a sua porcentagem.  
***
### Porcentagem de filmes e de series lancadas em determinado ano
Esta análise faz o cálculo da porcentagem de obras lançadas em um determinado ano. A quantidade de filmes e séries também é mostrado.  
O ano é dado pelo usuário.  
# Outras operações
### Ler arquivo
Ler o arquivo CSV onde estão os dados.  
Os dados são armazenados nas árvores AVL e BST.
***
### Inserir novo filme/serie
Opção de inserir nova obra nas árvores.  
Todas as informações necessárias são solicitadas antes de inserir nas árvores, para manter o padrão.  
***
### Procurar por filme/serie
Opção de procurar por uma obra nas árvores.  
Nesta opção, é impresso o tempo para fazer a busca um cada árvore.  
O ID de uma obra é solicitado para realizar a busca.  
Em teoria, a *AVL* seria mais rápida devido a menor altura que ela possui. Entretanto, dependendo do ID fornecido, a BST pode ser **mais rápida** ou **igualmente rápida** na busca.  
***
### Remover um filme/serie
Opção de remover um filme/serie.  
O ID de uma obra é solicitado.  
***
### Exibir as alturas das arvores
Opção de mostrar as alturas das árvores AVL e BST.  
***
### Salvar no arquivo
Opção de salvar o conteúdo da árvore AVL em um novo arquivo CSV.  
O nome deste arquivo é: arquivo_saida.csv  
# Executar o executável
1. Tenha um compilador de C++ instalado. Caso não tenha, siga as instruções da página do VS Code: [Using GCC with MinGW](https://code.visualstudio.com/docs/cpp/config-mingw).
2. Clone o repositório.
3. Execute o programa com o comando: _.\main.exe_. **Adendo**: é possível que a execução demore para começar devido à quantidade de arquivos necessários.
4. Caso o executável não esteja disponível, basta compilar os arquivos. Comando: _g++ main.cpp AVL.cpp BST.cpp NodeAVL.cpp NodeBST.cpp ProgramaNetFlix.cpp Utils.cpp -o main.exe_. **Adendo**: é possível que a compilação demore devido à quantidade de arquivos necessários.

# Alunos participantes
Eric Akio Uchiyamada  
Lucas Goulart de Farias Meres  
Oliver Kieran Galvão McCormack  
Pedro Loureiro Morone Branco Volpe  
Renan Tagliaferro  
Thiago Leandro Liporace  
