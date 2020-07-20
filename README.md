# Folha de respostas

## Javascript Questão 2:

### a) No import da api do google maps no index.html, para que servem as tags async e defer?
R: Ambas as tags sao responsaveis por carregar scripts externos sem comprometer a renderizacao da pagina HTML em si. O ASYNC faz o download dos scripts sem parar o processo de renderizacao da pagina, eh executado a a qualquer momento e em qualquer ordem, sera carregado de forma assincrona. O DEFER tambem eh responsavel pelo download mas eles so sao baixados apos a renderizacao da pagina estar completa e a ordem de download eh sempre respeitada, baixando um de cada vez.

### b) Para que serve o parâmetro &callback=initMap na url da api do google maps?
R: Serve para inicializar, de forma assincrona, uma nova instancia do mapa a ser visualizado. Assim que receber a resposta da API, o mapa eh carregado.

### c) O que acontece quando removemos o parâmetro &callback=initMap da url da api do google maps? Explique o porque.
R: O mapa nao eh inicializado pois nao eh chamado de uma forma assincrona na API. Deve-se esperar a resposta "ficar pronta" para devolver o mapa. Quando removemos o callback, nao esperamos a reposta e "voltamos" sem nenhuma resposta.

### d) Descreva pelo menos uma forma de como podemos fazer com que a aplicação funcione corretamente mesmo sem este parâmetro.
R: Uma outra forma de fazer com que aplicacao funcione sem este parametro, segundo a API do Google Maps, eh fazer um arquivo .js a parte e importa-lo para nosso arquivo index.html. A forma como esta sendo utilizado hoje eh Inline Loading, podemos utilizar o Dynamic Loading segundo a API do Google.

Fontes: https://developers.google.com/maps/documentation/javascript/overview#Loading_the_Maps_API

### e) Explique para que servem as seguintes tags do index.html: 
  `<link rel="manifest" href="manifest.json">
  <meta name="theme-color" content="">
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black">`

R: A tag LINK eh usada para importar um arquivo, seja ele CSS, json ou ate um icone para o favicon. Na TAG META eh definido algumas informacoes sobre o site, palavras-chaves para encontrar o site ou o view-port utilizado para mobile. No caso da aplicacao em questao, eh utilizado o link para referenciar um arquivo json Manifesto de Web App. A tag meta name="theme-color" serve para alterar a cor do tema que envolve o site. o name="apple-mobile-web-app-capable" fala que o site possa ou não ser executada em modo tela cheia em um dispositivo Apple, dependendo do valor que está dentro do atributo content. name="apple-mobile-web-app-status-bar-style" é responsável por estilizar a barra de progresso de um site quando o mesmo aberto por um dispositivo Apple.

### f) Está aplicação pode ser considerada um PWA? Em caso negativo, explique o que falta para que seja.
R: Embora tenha alguns conceitos, como as tags acimas utilizadas para o mobile, nao pode ser considerado uma PWA. Para ser considerado uma PWA, a aplicacao deve utilizar mais recursos, nao somente se consumir de um recurso da API do Google Maps.


## Angular Questão 4:

### a) Para que serve o método ngOnInit, quais são os outros métodos do Angular lifecycle hooks e para que servem?
R:

### b) Neste projeto, estamos usando os componentes gráficos da versão 4 da biblioteca gráfica do Ionic. Nesta versão, os componentes são Web Components. Explique o que são Web Components e explique quais são as vantagens deles.
R: 

### c) Para que serve a tag ngFor do angular?
R:


### d) O que o codigo abaixo representa no arquivo list.page.ts?
`legends: Array<string> = []`
R

### e) Como funciona a api Events do Ionic? Para que serve?
R: 

### f) O que é flexbox? Para que servem as tags ion-grid, ion-row, ion-col? Quais as vantagens em utilizálas?
R: 

## Angular Questão 6:

### a) Quais foram os problemas que você identificou?
R:

### b) Ordene os problemas por ordem de criticidade, ou seja, liste todos os problemas encontrados na ordem de quais deveriam ser corrigidos primeiro em um cenário onde devessemos priorizar as correções.
R:

### c) Justifique a ordem proposta no item anterior em termos de impacto para os usuários e dificuldade para corrigir o problema.
R: 

### d) Para que servem os comandos async e await, encontrados na função presentLoading do arquivo home.page.ts?
R: o Async serve para identificar que a funcao eh assincrona e o Await serve para identificar que uma chamada a outra funcao ou um uma funcao de outro componente pode demorar para responder, sendo assim, utilizamos o await para retornar a resposta quando a mesma estiver pronta. 

### e) Quais as vantagens de utilizar async/await em códigos javascript/typescript?
R: A vantagem eh que se pode usar funcoes assincronas em codigo sincrono. Podemos consumir qualquer recurso de API e obter a resposta quando a mesma estiver "pronta". Isso nao acaba travando sua aplicacao e fazendo a mesma ficar em esper.

### f) Explique para que serve a seguinte lib encontrada no arquivo home.page.ts import * as _ from 'lodash';
R:
