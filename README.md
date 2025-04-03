

# 3DS-A
## Kauê Parente Moretto
# Codigo 
``` html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fatorial e Número Primo</title>
</head>

<body>
    <h2>Calculadora de Fatorial e Verificador de Número Primo</h2>

    <label for="numero">Digite um número:</label>
    <input type="number" id="numero">
    <button onclick="calcular()">Calcular</button>

    <p id="resultado"></p>

    <script>
    // Função para calcular o fatorial de um número de forma recursiva
        function calcularFatorial(n) {
            if (n === 0) {
                return 1; // O fatorial de 0 é 1
            } else {
                return n * calcularFatorial(n - 1);
}
}

// Função para verificar se um número é primo
    function verificarNumeroPrimo(numero) {
        if (numero <= 1) {
        return false; // Números menores ou iguais a 1 não são primos
}
    for (let i = 2; i < numero; i++) {
        if (numero % i === 0) {
        return false; // Se for divisível por outro número além de 1 e ele mesmo, não é primo
}
}
    return true; // Se passou pelo loop sem encontrar divisores, é primo
}

// Função principal que calcula e exibe os resultados na página
    function calcular() {
        let numero = parseInt(document.getElementById("numero").value); // Obtém o número inserido pelo usuário
        let fatorial = calcularFatorial(numero); // Calcula o fatorial do número
        let primo = verificarNumeroPrimo(numero); // Verifica se o número é primo

// Exibe os resultados na página
    document.getElementById("resultado").innerHTML =
    " O fatorial de " + numero + " é " + fatorial + "<br>" +
    "O número " + numero + (primo ? " é primo." : " não é primo.");
}
</script>
</body>

</html>
``` 

# Respostas 

## 1. O que mudou no código após a formatação e adição de comentários?
## A formatação melhorada torna o código mais organizado e fácil de entender. Comentários ajudam a compreender a lógica sem necessidade de análise profunda.



## 2. Como a rastreabilidade auxilia na compreensão e manutenção do código?
## A rastreabilidade permite que futuros desenvolvedores entendam rapidamente as funcionalidades do código, reduzindo o tempo de manutenção e facilitando a depuração de erros.


## 3. Quais práticas você considera essenciais para garantir um código bem documentado?
- Uso de indentação e espaçamento adequados.

- Comentários explicativos em trechos importantes.

- Nomeação clara de variáveis e funções.

- Documentação externa (como este arquivo Markdown).

## 4. Qual a importância do uso do Markdown na documentação do código?
## O Markdown facilita a criação de documentações organizadas e legíveis, permitindo que desenvolvedores consultem rapidamente informações essenciais sobre o código.

## 5. Como a padronização e boas práticas de projeto facilitam a manutenção e escalabilidade de sistemas?
## A padronização evita ambiguidades e torna a colaboração mais eficiente. Com boas práticas, é possível escalar o sistema sem comprometer a legibilidade e funcionalidade do código
