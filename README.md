## Criação de uma task (Rota: POST - /tasks):

Para criar uma nova task, você pode criar uma rota que lida com a requisição POST. Extraia os campos title e description do corpo da requisição e crie um novo objeto de task, preenchendo os campos obrigatórios, como id, created_at e updated_at. Em seguida, salve a task no banco de dados.

## Listagem de todas as tasks (Rota: GET - /tasks):

Para listar todas as tasks, implemente uma rota que recupera todas as tasks do banco de dados. Você também pode adicionar a funcionalidade de filtrar as tasks com base nos campos title e description usando query parameters.

## Atualização de uma task pelo id (Rota: PUT - /tasks/:id):

Para atualizar uma task existente, crie uma rota que lide com requisições PUT, onde você receberá o id no parâmetro da URL e o objeto de atualização no corpo da requisição. Verifique se o id corresponde a uma task no banco de dados e, em seguida, atualize os campos apropriados.

## Remover uma task pelo id (Rota: DELETE - /tasks/:id):

Crie uma rota para lidar com as requisições DELETE, onde você receberá o id no parâmetro da URL. Verifique se o id pertence a uma task no banco de dados e, se for o caso, remova a task correspondente.

## Marcar pelo id uma task como completa (Rota: PATCH - /tasks/:id/complete):

Para marcar uma task como completa ou reverter o status, crie uma rota que lide com requisições PATCH. Você precisará verificar se o id corresponde a uma task no banco de dados e, em seguida, atualizar o campo completed_at para refletir o novo status.

### Importação de tasks em massa por um arquivo CSV:

Para lidar com a importação de tasks através de um arquivo CSV, siga as instruções fornecidas na página de explicação sobre a criação via CSV com Stream. Basicamente, você precisará ler o arquivo CSV, analisar os dados e criar/atualizar as tasks correspondentes no banco de dados.
