# Teste_calculadora
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Somando Números</title>
    <style>
        body{ font: normal 17pt Arial; 
        }
        input {
            font: normal 17pt Arial;
            width: 150px;
        }
        
    </style>
</head>
<body>
    <h1>Somando Valores</h1>
    <input type="number" name ="txtn1" id="txtn1"> +
<input type="number" name = "txtn2" id = "txtn2">
<input type="button" value="Somar" onclick ="somar()">
<div id="res">Resultado da soma</div>
<br>
<br>
<input type="number" name = "txtn3" id= "txtn3">  x 
<input type="number" name = "txtn4" id = "txtn4">
<input type="button" value="Multiplicar" onclick="multiplicar()">

<div id ="res2">Resultado da multiplicação</div>

<style>
    body { font: normal 18pt Arial;
    }
    div#res { 
        margin-top: 20px;
    }
    div#res2 {
        margin-top: 20px;
    }
</style>

<script>
    function somar() {
        var tn1 = window.document.getElementById('txtn1')
        var tn2 = window.document.querySelector('input#txtn2')
        var res = window.document.getElementById('res')
        var n1 = Number(tn1.value)
        var n2 = Number(tn2.value)
        var s = n1 + n2
        res.innerHTML = `A soma entre ${n1} e ${n2} é igual a <strong>${s}</strong>`
        }
     function multiplicar() {
            var tn3 = document.getElementById('txtn3')
            var tn4 = document.getElementById('txtn4')
            var res2 = document.getElementById('res2')
            var n3 = Number(tn3.value)
            var n4 = Number(tn4.value)
            var d = n1 * n2 
            res2.innerHTML = `A multiplicação entre ${n3} e ${n4} é igual a <strong>${d}</strong>`

        }
</script>
</body>
</html>
