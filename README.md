# DioLab-AzureAISearch


Passo a passo Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados.


Nesse passo a passo vamos ver como podemos utilizar a Inteligência Artificial para buscas cognitivas.


Passo 1 - Crie um recurso, procure por AI Search.

![criando um recurso](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/b000dae3-8ca8-44f7-af49-549ce3e75749)

Passo 2 - Crie um novo recurso, dessa vez procurando por AI Service.


Passo 3 - Crie uma conta de armazenamento, escolhendo a opção Storage Account.

![storage account](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/22bf3b25-0e5a-4ba0-8750-9afd63303cc7)

Passo 4 - Configure o Storage account, habilite a opção Allow Blob anonymous access e depois confirme.

![configuração do storage account](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/9d076b8b-3628-4c83-8735-6c6ea0b2dcaa)


Passo 5 - Crie um novo container.

![criando novo container](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/14dc8eeb-7e55-4fa9-befa-8fa7ecf5baec)


Passo 6 - Selecione o container criado e clique em  upload. Para esse desafio, foi feito o upload dos seguintes dados que estão na documentação da Microsoft Azure: https://aka.ms/mslearn-coffee-reviews.

![upload dos arquivos no container](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/468775ae-3389-4f3e-927d-2ada6b2cf125)


Passo 7 - Volte ao AI Search e selecione o serviço criado.

![ai search](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/590d57b7-f7f2-43e7-b24f-d3a2a4bf340e)


Passo 8 - selecione o serviço criado e clique na opção import data.


![importandio dados no AI search](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/28cd37c0-27dc-4736-a54f-751235635653)

![importando data no AI Search](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/e662747c-8eb7-4f41-a6b3-b6ad6988ebd8)


Passo 9 - Clique na opção choose an existing conection e selecione o container criado.

![selecionando uma conexão existente](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/68655564-ce40-4f9d-9179-2f6937f6bb66)


Passo 10 - Em add cognitive skills, vá na aba Attach AI Services e selecione o recurso criado.

![Attach AI Services](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/5452d0e1-b6f5-4afd-aff3-a72ae3dcc42a)


Passo 11 - Em add cognitive skills, vá na aba Add enrichments, preencha os campos conforme a imagem abaixo.

![add enrichments](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/f2102909-c032-4a75-a21b-4daa93b340c8)


Passo 12 - Em Save enrichments to a knowledge store, selecione a caixa Image Projections e clique em Choose an existing connection

![saver enrichments to a knowledge store](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/b482a811-819a-4978-a232-0625b43d9f89)


Passo 13 - Selecione o recurso criado e selecione as opções conforme a imagem abaixo.

![save enrichments](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/a907d616-43f1-4f4a-882f-61d1b1923842)


Passo 14 - Na aba Customize target index, prreencha conforme abaixo.

![import data](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/f40248cc-f5bd-4c2f-ad04-f01468f93c7c)


Passo 15 - Em Create an indexer , selecione a caixa Base-64 Encode Keys e clique em Submit.

![create an indexer](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/0248dbe0-677f-46b9-9226-05cda472fa0b)


Passo 16 - Volte ao AI Search e escolha a opção search explorer

![search explorer](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/c0b23686-c6d5-49a2-964a-114194a2bfe7)



Entrando no ambiente de pesquisa você pode colocar a query search=*&$count=true e ele vai pesquisar de onde as informações estão saindo


![search explorer index](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/4ea1b1dd-8ef1-4439-b205-35c65c2f5a59)


Usando a query search=locations:'Chicago' , você consegue saber qual a opinião dos clientes em relação a cafeteria na região de Chicago

![search sentimentos](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/bd065d59-1681-4bd2-ab08-f3f60b7e0dc9)


Com a query search=sentiment:'negative' , você consegue filtrar somente os sentimentos e opiniões negativas dos clientes

![search sentimento negativo](https://github.com/anamirannda/DioLab-AzureAISearch/assets/151754232/8505f290-4fe8-4f2a-8962-aca64b3a78f2)




Através desse serviço da Microsoft Azure, você pode analisar melhor o que os clientes do seu negócio estão sentindo, qual a opinião deles sobre o seu produto e serviço. Isso ajuda demais na criação de novas estratégias para a conversão de novos clientes e personalização de atendimento fidelizando aqueles que já fazem uso do que o seu negócio oferece.




