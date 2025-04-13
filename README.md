# calcularjuros

lembretes 

📌 1. Pegar valor do input
js
Copiar código
let nome = document.getElementById("nome").value;
Isso pega o que o usuário digitou num campo <input id="nome">.

.value = valor que foi escrito.

📌 2. Converter string para número
Tudo que vem de um input é texto (string). Se for fazer conta, tem que converter:

js
Copiar código
let numero = parseFloat(document.getElementById("numero").value);
parseFloat() transforma em número com vírgula.

Se quiser só número inteiro: parseInt().

📌 3. Mostrar o resultado na tela
js
Copiar código
document.getElementById("resultado").innerText = "Resultado: " + soma;
innerText (coloca texto dentro de uma tag como) <p id="resultado">.

📌 4. Função com botão
Você liga um botão a uma função assim:

html

Copiar código
<button onclick="somar()">Somar</button>

js
Copiar código
function somar() {
  let n1 = parseFloat(document.getElementById("n1").value);
  let n2 = parseFloat(document.getElementById("n2").value);
  let soma = n1 + n2;
  document.getElementById("resultado").innerText = soma;
}

📌 5. Condições
js
Copiar código
if (numero2 == 0) {
  alert("Não pode dividir por zero!");
} else {
  let resultado = numero1 / numero2;
}


📌 6. Try...catch (caso use eval ou erro)
js
Copiar código
try {
  let resultado = eval("10 + 2");
} catch (error) {
  alert("Erro na expressão");
}
