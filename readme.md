# Atividades da Lista 2 de Sistemas Operacionais 2022.1 💻📚

## PARTE 1 - THREADS

### 1.1. O programa em C usa a biblioteca de threads do linux para criar um thread pai que irá gerar 100 threads filhas, e na criação de cada thread irá ser dito um “olá” referente à thread criada no momento, e na finalização de cada thread será dito um “tchau” referente à thread que terminou o seu processo. Dessa forma, foi criada uma thread pai com o comando pthread_create, este comando retorna um valor 0 para uma criação bem sucedida de uma thread, e com isso foi feita um if para dizer que a thread foi ou não criada com sucesso. Seguindo o código, com a criação bem sucedida do thread pai, a função pthread_join aguarda o término do thread para que os processos de cada thread saiam em ordem. Portanto, usando a mesma lógica para a criação do thread pai, é criado um vetor de threads[N], em que N é 100, no topo do código para que dentro da função chamada pelo thread pai, seja executado um laço for com pthread_create para cada uma das N threads do vetor, e finalmente cada thread filha irá dizer um olá na sua criação e um tchau na sua finalização.

### 1.2. O algoritmo calcula o seno de x através da série de taylor usando a biblioteca de thread do linux. Este programa conta com quatro funções, uma que calcula o fatorial do denominador, outras duas funções que calculam o somatório de números positivos e negativos, e por fim a função main, que é a função principal, e lá é onde foram criados as threads. Ademais, a função “somador” é chamada pela thread “somadora” e a função “subtrator” é chamada pela thread subtratora. Assim como a função “factorial” é chamada em cada uma das funções somadoras. Dessa forma é criado duas variáveis globais que armazenam os valores dos somatórios das duas principais funções, e por fim os valores são somados na função main e é exibido para o usuário.

### 1.3. A última parte da seção de threads se trata de um algoritmo em C que usa a biblioteca de threads do linux para dividir entre duas threads a tarefa de calcular o número de números primos entre zero e um número digitado pelo usuário. Portanto, para isso foi implementado no código quatro funções, uma main que irá criar os threas, obter a entrada do número fornecido pelo usuário e mostrar a quantidade de números primos, duas funções “counters” que irão conter um laço de repetição para percorrer os valores de 0 até N/2 e de ((N/2)+1) até N, assim como irão chamar a função “ifPrimo” que irá dizer se o número informado é ou não primo e irá imprimir aquele valor na tela.

## PARTE 2 - ESCALONAMENTO

## PARTE 3 - SISTEMA DE ARQUIVOS

### obs: Para mais informações, porfavor ler o pdf na pasta docs

### Membros: Marcos Vinicius e Yann Lucca
