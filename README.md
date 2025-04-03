# Markdown

## Diogo Lugano Xavier Farrapo - 3 DS A

# Aprendendo Markdown
## Aprendendo Markdown

Aplicando **Negrito** em Markdown

Aplicando *Itálico* em Markdown

> Texto em caixa
>
> Exemplo

# Calculadora de Fatorial
``` HTML
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
        // Função para calcular o fatorial.
        function calcularFatorial(n) {
            if (n === 0) {
                return 1;
            } else {
                return n * calcularFatorial(n - 1);
            }
        }
        // Função para verificar se o número é primo.
        function verificarNumeroPrimo(numero) {
            if (numero <= 1) {
                return false;
            }
            for (let i = 2; i < numero; i++) {
                if (numero % i === 0) {
                    return false;
                }
            }
            return true;
        }
        // Função para calcular.
        function calcular() {
            let numero = parseInt(document.getElementById("numero").value);
            let fatorial = calcularFatorial(numero);
            let primo = verificarNumeroPrimo(numero);
            document.getElementById("resultado").innerHTML =
                "O fatorial de " + numero + " é " + fatorial + "<br>" +
                "O número " + numero + (primo ? " é primo." : " não é primo.");
        }
    </script>
</body>

</html>
```

# Respostas
1. Após a identação do código, o código fica mais organizado, e os comentários ajudam a esclarecer algumas partes do código.
   
2. A rastreabilidade permite identificar a origem e evolução de cada parte do código, facilitando a depuração, atualização e integração de novas funcionalidades sem comprometer a estabilidade do sistema.
   

3. Práticas essenciais são o uso de comentários claros e objetivos. Uma estrutura mais organizada e modular do código.

4. Com o Markdown, podemos criar documentos organizados e objetivos, já que a maneira de documentar as coisas são bem simples.

5. A padronização garante um desenvolvimento eficiente, uma separação de responsabilidades e modularização torna o código mais flexível, e isso facilita futuras correções.
