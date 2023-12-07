## Proposta
Projetos de equipes de 1 à 2 pessoas para entregar até o dia 14/12 (valendo a nota N2)

Projeto 1 (inglês)


Projeto do site: https://fun-javascript-projects.com/course

Neste site você encontrará vários projetos em Javascript com ví­deos explicando como cada projeto foi feito, passo a passo
No entanto, os códigos fontes do projeto podem ser encontrados no github, mais especificamente, na página: https://github.com/chrisdixon161/fun-javascript-projects.com


Após clonar e executar o web app na sua máquina - para garantir que ele está funcionando - proceder com as modificações listadas abaixo.

Para este trabalho, você deverá modificar o projeto nº6 (MP3 Player), conforme itens abaixo.

1) Substituir a imagem do fone de ouvido por uma outra de seu gosto. Crie sua própria, se você souber (usando a tag svg, por exemplo) ou procure uma na internet. Neste caso, busque por "royalty free images", de preferência imagens vetoriais e com fundo transparente.

2) Modificar a cor de fundo do player para a cor de sua preferência

3) Modificar a fonte usada no player para a de sua preferência

4) Modificar as músicas com as suas preferidas. 

5) Exibir na lista de músicas o título apenas, sem a extensão do arquivo.

6) Explique, com suas próprias palavras, o que faz o seguinte trecho de código:

``` bash
const createSongList = () => {
  const list = document.createElement("ol");
  for (let i = 0; i < songs.length; i++) {
    const item = document.createElement("li");
    item.appendChild(document.createTextNode(songs[i].slice(0,-4)));
    list.appendChild(item);
  }
  return list;
};
```

7) Modifique o código para quando você clicar sobre a barra de progresso, a música avançar para o ponto correspondente

## Resposta
6) 
- Primeiro ele cria um elemento *HTML* chamado ("ol") que é uma *lista ordenada dentro da variável "list".*

- Depois ele entra em um *for loop* de acordo com o tamanho da sua lista de músicas

- Depois ele cria outro elemento *HTML* chamado ("li") dentro da variável "item" que é o elemento que fica dentro do ("ol")

- Depois disso ele adiciona o nome de cada iteração da *Array* "songs" dentro de "item" usando o createTextNode

- E por fim ele põe o "item" (li) na "list" (ol)

``` bash
<ol>
    <li>My_way_-_Frank_Sinatra.mp3</li>
</ol>
``` 
