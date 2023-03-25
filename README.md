API Básica em Django
Esta é uma API básica em Django que permite a criação, listagem, atualização e exclusão de alunos.

Endpoints
A API tem os seguintes endpoints:

GET /alunos/
Retorna uma lista de todos os alunos cadastrados.

Exemplo de resposta:

perl
Copy code
```
[
    {
        "id": 1,
        "nome": "João",
        "idade": 20,
        "email": "joao@email.com"
    },
    {
        "id": 2,
        "nome": "Maria",
        "idade": 22,
        "email": "maria@email.com"
    },
    
]
```
GET /alunos/:id/
Retorna as informações de um aluno específico.

Exemplo de resposta:

```
{
    "id": 1,
    "nome": "João",
    "idade": 20,
    "email": "joao@email.com"
}
```
POST /alunos/
Cria um novo aluno.

Exemplo de corpo da requisição:

```
{
    "nome": "José",
    "idade": 25,
    "email": "jose@email.com"
}
```
PUT /alunos/:id/
Atualiza as informações de um aluno específico.

Exemplo de corpo da requisição:


```
{
    "nome": "João da Silva",
    "idade": 21,
    "email": "joao.silva@email.com"
}
```
DELETE /alunos/:id/
Exclui um aluno específico.

Deploy
A API está atualmente em produção no serviço PythonAnywhere e pode ser acessada em https://neitaloengdev.pythonanywhere.com/alunos/?format=json.

Autor
Italoengdev
