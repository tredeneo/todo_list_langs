projeto de avaliação para a empresa mindtech 

# feedback
` gostaria de dizer que gostei da sua abordagem para o projeto, resolvendo de maneira simples e eficaz. Porém gostaria de destacar alguns pontos aqui: Você poderia ter usado um "id" nas tarefas, ao invés de identificar elas pelo título. Assim seria mais fácil de consumir a sua API. Outra coisa é que a rota "GET /tarefa" retorna apenas a última tarefa registrada, e não uma escolhida.`

# requisitos
* python > 3.6
* flask

é possivel rodar com 
```
python principal.py
```
ou
```
python3 principal.py
```

não defini uma url padrão então o endereço pode variar do sistema e o que tiver rodando nas portas mas no geral vai abrir em `http://localhost:5000/` ou `http://127.0.0.1:5000`

# guia de uso da API
### /tarefas
* GET
* lista todas as tarefas cadastradas

### /tarefa
* GET
* lista uma  tarefa
```json
{
	"titulo":"titulo da tarefa", 
}
```
### /tarefa
* POST
* cadastrar tarefa
```json
{
	"titulo":"titulo da tarefa",
	"descricao":"descricao da tarefa"
}
```

### /tarefa
* DELETE
* exclui uma tarefa cadastrada
```json
{
	"titulo":"titulo da tarefa",
}
```

### /concluir_tarefa	
* POST
* conclui uma tarefa
```json
{
	"titulo":"titulo da tarefa",
}
```

### /atualizar_tarefa 	
* POST
* atualiza uma tarefa
```json
{
	"titulo":"titulo atual da tarefa",
	"novo_titulo":"novo titulo que sera atribuido a tarefa",
	"nova_descricao":"nova descrição que sera atribuida a tarefa"

}
```
