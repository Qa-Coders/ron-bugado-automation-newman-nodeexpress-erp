# Teste Diretoria Ron Bugado

## Caminho Feliz

### Login_Sucesso 
- Verifica se o Status Code é 200
- Valida mensagem de sucesso

### Diretoria_Sucesso
- Verifica se o Status Code é 201
- Valida se nameBoard é o mesmo enviado no body
- Verifca se o status da Diretoria é true
- Verifica se o codeBoard é retornado 
- Verifica se o id é retornado

### Diretoria_GetList
- Verifica se o Status Code é 200

### Diretoria_GetId
- Verifica se o Status Code é 200
- Verifica se o id retornado é o enviado
- Verifica se o nameBoard enviado está correto

### Diretoria_Count
- Verifica se o Status Code é 200
- Verifica o total de registros retornados

### Diretoria_Update
- Verifica se o Status Code é 200
- Verifica se o id retornado é o enviado
- Verifica se o nameBoard enviado está correto

### Status_False_Success
- Verifica o Status Code 202
- Validação da mensagem de sucesso

### Busca_Dire_Inativada
- Verifica o Status Code 200

### Status_True_Success
- Verifica o Status Code 200
- Verifica mensagem de cadastro atualizado
- Verifica se o Status retornou true

## Exceções

###  PUT POST Dire_Vazio
- Valida Status Code 400
- Valida mensagem de erro "O campo diretoria é obrigatório"

### PUT POST Dire_null
- Valida Status Code 400
- Valida mensagem de erro " O campo diretoria é obrigatório"

### PUT POST Dire_max_50caracteres
- Valida o Status Code 400
- Valida mensagem de erro " O campo diretoria possuir 50 caracteres"

### PUT POST Dire_so_numeros
- Valida o Status Code 400
- Valida mensagem de erro "O campo diretoria só pode conter letras e o caractere especial & "

### PUT POST Dire_ja_cadastrada
- Valida o Status Code 409
- Valida a mensagem de erro "Não é possível cadastrar esse registro. Diretoria já cadastrada no sistema."

### PUT POST Dire_so_cara_especiais
- Valida o Status Code 400
- Valida mensagem de erro "O campo diretoria só pode conter letras e o caractere especial & "

## Sem Token

### POST Cadastro_semToken
- Valida o Status Code 403
- Valida a mensagem de erro "No token provided".

### GET DiretoriaList_semToken
- Valida o Status Code 403
- Valida a mensagem de erro "No token provided".

### GET Diretoria_GET_ID_semToken
- Valida o Status Code 403
- Valida a mensagem de erro "No token provided".

### GET Diretoria_Count_semToken
- Valida o Status Code 403
- Valida a mensagem de erro "No token provided".

### PUT Alterar_Cadastro_semToken
- Valida o Status Code 403
- Valida a mensagem de erro "No token provided".

##  Token Inválido

### POST Cadastro_TokenInválido
- Valida o Status Code 403
- Valida a mensagem de erro "Failed to authenticate token.".

### GET DiretoriaList_TokenInválido
- Valida o Status Code 403
- Valida a mensagem de erro "Failed to authenticate token.".

### GET Diretoria_GET_ID_TokenInválido
- Valida o Status Code 403
- Valida a mensagem de erro "Failed to authenticate token.".

### GET Diretoria_Count_TokenInválido
- Valida o Status Code 403
- Valida a mensagem de erro "Failed to authenticate token.".

### PUT Alterar_Cadastro_TokenInválido
- Valida o Status Code 403
- Valida a mensagem de erro "Failed to authenticate token.".












