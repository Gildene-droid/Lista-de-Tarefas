<!DOCTYPE html>
<html lang="pt-BR">

<head>
<meta charset="UTF-8">
<title>Lista de Tarefas</title>
</head>

<body>

<h1>Minha Lista de Tarefas</h1>

<input type="text" id="tarefa" placeholder="Digite uma tarefa">
<button onclick="adicionarTarefa()">Adicionar</button>

<ul id="lista"></ul>

<script>

function adicionarTarefa() {

let tarefa = document.getElementById("tarefa").value;

if (tarefa === "") {
alert("Digite uma tarefa");
return;
}

let li = document.createElement("li");
li.innerText = tarefa;

document.getElementById("lista").appendChild(li);

document.getElementById("tarefa").value = "";

}

</script>

</body>
</html>
