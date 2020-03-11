# Cyberlabs
### **Beat Human Performance!**

---

Esse código foi produzido como parte do processo de seleção da Cyberlabs, utilizando a plataforma "Google Colab"; para visualização do mesmo, basta seguir o link no arquivo. 
Para execução na plataforma, crie uma cópia do arquivo do colab e faça o upload do CSV(dataset) para o mesmo.
Primeiro execute todo o código em "Analize e preparo do dataset" e então, o metodo que preferir.

---

## Processos de criação e execução ##

---

Decidi fazer o teste no Google colab, pra ter acesso ao mesmo em qualquer lugar e testar separadamente a execução de cada bloco.

Meu primeiro desafio foi entender a estrutura de cada feature e se alguma coisa no dataset poderia prejudicar o treinamento. Comecei a comentar cada parte do código, não apenas pra facilitar o entendimento,
mas pra me guiar na hora de fazer as alterações. O primeiro passo foi fazer a divisão e analize do dataset, bem como estruturação. Após organizar todos os passos, fiz o primeiro treinamento e predileção utilizando árvore de decisão.
Analizei os resultados e parti para testar outros metodos de aprendizado. Minha segunda escolha foi o KNN, no qual consegui aumentar um pouco mais a acurácia; Aqui normalizei os dados utilizando StandardScaler. Utilizei 
então a regressão logistica, e cheguei no famigerado Random forest,utililzando um GridSearch para decidir os melhores parametros. Tambem utilizei o metodo Naive Bayers, que não me gerou grandes alterações.

Por último decidi utilizar o metodo XGboost, até então um metodo que eu conhecia menos que os outros. Consegui um resultado melhor que com os outros, por tanto considero o método principal do modelo; Tive um pouco de 
dificuldades com a hiper-parametrizaçao do mesmo, pois demorava muito. finalmente depois de alguns testes, consegui ajustar manualmente da melhor maneira, conseguindo uma Acurácia de 84%.
gerei um grafico no final de importancia de cada feat, para fins de analize do xgboost em comparação com o grafico inicial por idade.

Obs: Usei inicialmente o Random State: Default, então foi bem triste ver a acurácia cair ao setar o RS pra 42. mas creio que me recuperei bem do choque.