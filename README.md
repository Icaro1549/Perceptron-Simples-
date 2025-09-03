# Perceptron-Simples-
Um perceptron é o fundamento de uma ia, o perceptron copia o funcionamento de um neurônio humano. Ele é bastante usado pra resolver problemas simples e binários, não muito indicado pra problemas complexos.

# Perceptron 

O que é um perceptron é qual sua importância pra inteligência artificial:

Um perceptron é um neurônio digital criado em 1958. Em uma tentativa de criar um cérebro artificial, os cientistas tentaram copiar o funcionamento do cérebro humano, e assim recriaram os neurônios de forma artificial, causando o surgimento do perceptron. O perceptron foi um dos pilares para o desenvolvimento das inteligências artificiais, assim como para a compreensão de uma rede neural, um pilar fundamental para o funcionamento das inteligências artificiais que conhecemos hoje em dia.

Funcionamento:

O perceptron funciona de forma linear e binária, separando as coisas em duas coisas. Sim/não, Verdadeiro/Falso, 0/1. Por isso ele é chamado de classificador linear. Ele faz distinção binária das coisas, baseado nos dados que obteve. Seu principal defeito também é esse, devido a sua linearidade, ele não consegue resolver problemas muito complexos.

Código:

O código de um perceptron básico é relativamente simples, você oferece a ele alguns valores, atribui peso a eles, e oferece um limiar. Após isso você fala que tipo de conta ele tem que fazer e compara o resultado baseado em seu limiar, se for maior, ele dirá um resultado, se for menor, ele falará outro resultado.

Exemplos de perceptron: 

Um exemplo extremamente comum de perceptron que usados no dia a dia é um sensor simples de ar condicionado/aquecedor. Ele recebe os sinais do ambiente como temperatura do ambiente, compara se tá muito quente ou frio e dá um resultado podendo ser o acionamento do ar condicionado pra resfriar ou do aquecedor pra aquecer


    Código de um perceptron simples 


    def main():

    print("Olá usuário!")
    print("O resultado do input é: ", perceptron_input([1,2,3], [0.1,0.2,0.3], 0.4))
    print("O resultado do perceptron é: ", perceptron_output([1,2,3], [0.1,0.2,0.3], 0.4))

    def perceptron_input(inputs, weights, bias): 

    weighted_sum = sum(i*w for i,w in zip(inputs,weights)) 

    return weighted_sum + bias 

    def perceptron_output(inputs, weights, bias):

    return 1 if perceptron_input(inputs, weights, bias)>= 0 else 0


    if __name__ == "__main__":

    main()
    
