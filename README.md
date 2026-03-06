<!DOCTYPE html>
<html>
<head>
<title>Lista de Tarefas</title>
</head>

<body>

<h1>Minha Lista de Tarefas</h1>

<input type="text" id="tarefa" placeholder="Digite uma tarefa">
<button onclick="adicionarTarefa()">Adicionar</button>

<ul id="lista"></ul>

<script>

function adicionarTarefa() {
    var tarefa = document.getElementById("tarefa").value;

    var li = document.createElement("li");
    li.textContent = tarefa;

    document.getElementById("lista").appendChild(li);

    document.getElementById("tarefa").value = "";
}

</script>

</body>
</html>
