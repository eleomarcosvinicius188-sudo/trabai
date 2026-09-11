# trabai
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Validação de Produtos</title>
</head>
<body>

    <h1>Calculadora de Desconto</h1>

    <script src="javas.js"></script>

</body>
</html>

function calcularProduto(nome, preco, desconto) {
    const valorDesconto = preco * desconto / 100;
    const valorFinal = preco - valorDesconto;

    alert(
        `${nome}\n` +
        `Preço: R$ ${preco.toFixed(2)}\n` +
        `Desconto: R$ ${valorDesconto.toFixed(2)}\n` +
        `Valor final: R$ ${valorFinal.toFixed(2)}`
    );
}

// Produto 1
const produto1 = prompt("Nome do 1º produto:");
const preco1 = parseFloat(prompt("Preço do produto:").replace(",", "."));
const desconto1 = parseFloat(prompt("Desconto (%):").replace(",", "."));

calcularProduto(produto1, preco1, desconto1);

// Produto 2
const produto2 = prompt("Nome do 2º produto:");
const preco2 = parseFloat(prompt("Preço do produto:").replace(",", "."));
const desconto2 = parseFloat(prompt("Desconto (%):").replace(",", "."));

calcularProduto(produto2, preco2, desconto2);

// Produto 3
const produto3 = prompt("Nome do 3º produto:");
const preco3 = parseFloat(prompt("Preço do produto:").replace(",", "."));
const desconto3 = parseFloat(prompt("Desconto (%):").replace(",", "."));

calcularProduto(produto3, preco3, desconto3);
