
# Instalando o  Newman e HTML Reporters:

Como pré requisito, você deve ter instalado o node.js na sua máquina.

Abra o cmd e digite:

``` npm install -g newman ```

Assim que completar a instalação, digite os seguintes comandos:

```npm install -g newman-reporter-html```


```npm install -g newman-reporter-htmlextra```


Já com o newman instalado, podemos dar prosseguimento a geração do dashboard.

Devemos efetuar o export da collection e do enviromment utilizado.

## Export collection

![NPM](https://cdn.discordapp.com/attachments/1016144040091197501/1016360196873928784/exportCollection.jpg)




## Export Enviromment

![NPM](https://cdn.discordapp.com/attachments/1016144040091197501/1016360197142368296/exportEnviromment.jpg)


Feito isso, abrindo um cmd na pasta que salvou os Exports , você deve executar o seguinte comando:

``` newman run YourCollectionName.json -e YourEnvironment.json -n 2 -r htmlextra ```

Substituindo YourCollectionName.json pelo nome do seu arquivo json da sua collection e 
Substituindo YourEnvironment.json pelo nome do seu arquivo json da sua environment.

Logo após a execução do comando os testes serão executado pelo newman e irão gerar uma pasta chamada newman dentro da pasta de origem.
Um arquivo .html será gerado, onde contém o dashboard de execução dos testes.





# ***Dashboard do Newman***

![NPM](https://cdn.discordapp.com/attachments/1016144040091197501/1016357144787943454/Newman.jpg)
