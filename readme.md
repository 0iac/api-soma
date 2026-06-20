# TDE: API REST com Flask (Integração Cliente-Servidor)

## Este repositório contém o código desenvolvido para o Trabalho Discente Efetivo (TDE) do Módulo 2 (Aplicação para ambiente WEB) do curso de Bacharelado em Cibersegurança da Universidade Federal de Uberlândia (UFU).

## O objetivo do projeto foi construir do zero uma API em Flask (servidor) e scripts em Python (clientes) para exercitar os conceitos de arquitetura Web, protocolos HTTP, integração cliente-servidor e segurança.

## O projeto foi evoluído em 4 etapas (horários):

 - Horário 1: Servidor Flask com rota inicial "GET /api/soma" recebendo parâmetros via URL (query string) e retornando o resultado em formato JSON.
 - Horário 2: Script cliente em Python (cliente.py) utilizando a biblioteca "requests" para consumir a rota GET de forma automatizada.
 - Horário 3: Rota "POST /api/soma" que aceita dados estruturados no corpo da requisição (JSON) e faz a leitura de metadados customizados no cabeçalho (X-Cliente).
 - Horário 4: Rota protegida ("GET /api/protegido") com validação de controle de acesso usando "Bearer Token" no cabeçalho "Authorization", tratando cenários de sucesso (200 OK) e erro (401 Unauthorized).

## Como executar

### 1 Clone o repositorio
`git clone [https://github.com/0iac/api-soma.git](https://github.com/SEU_USUARIO/api-soma.git)
cd api-soma`

### 2 Crie e ative o ambiente virtual
`python -m venv .venv`
`venv\Scripts\activate.bat`

### 3 Instale as dependências
`pip install flask requests` 

### 4 Ative o servidor
`python servidor.py`

### 5 Em outro terminal execute os demais codigos dentro da pasta "api-soma"
`python cliente.py`
`python cliente_post.py`
`python cliente_token.py`

## AUTORES
Caio Soares Fernandes

## PROFESSORES
Alan Petrônio, Marcelo Rodrigues, Kil Jin e Renato Carrijo (FEELT/UFU)
