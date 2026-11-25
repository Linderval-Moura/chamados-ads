# API de Chamados-ADS

**Estudante:** Linderval Moura Matias

## Objetivo do Projeto
Desenvolver a estrutura inicial da API REST de chamados ADS desenvolvida em Python com Flask, implementando a rota raiz (`GET /`) para verificação de funcionamento do serviço.

## Instalação das Dependências
Com o gerenciador de pacotes `uv` instalado (`pip install uv`), execute o comando abaixo na raiz do repositório para criar o ambiente virtual e instalar as dependências exatas definidas no `uv.lock`:

```bash
uv sync --locked
```

## Como executar a aplicação
Para iniciar o servidor Flask no ambiente de desenvolvimento (Codespaces), execute:

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

## Como acessar a rota inicial e qual resposta esperar
Com a aplicação em execução, acesse `http://localhost:5000/` pelo navegador ou faça uma requisição via terminal utilizando `curl`:

```bash
curl -i http://localhost:5000/
```


A resposta esperada possui status HTTP `200 OK`, cabeçalho `Content-Type: application/json` e o seguinte corpo JSON:

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```