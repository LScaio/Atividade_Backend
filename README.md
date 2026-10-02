# Projeto Web - LH Pets (Protótipo 1)

Aplicação back-end em ASP.NET Core (C#) com as rotas:

| Rota | Descrição |
|------|-----------|
| `/` | Exibe a versão inicial do projeto: **LH Pets - Protótipo 1** |
| `/index` | Redireciona para a página estática `wwwroot/index.html` (front-end) |
| `/listaClientes` | Exibe a lista de clientes cadastrados no banco `vendas` (SQL Server) |

## Como executar

1. No SQL Server Management Studio, conecte com o login `sa` / senha `12345` e execute o script `vendas.sql`.
2. Confira a string de conexão em `Banco.cs` (servidor `localhost\SQLEXPRESS`).
3. No terminal, na pasta do projeto:
   ```
   dotnet restore
   dotnet run
   ```
4. Abra o endereço exibido no terminal e acesse `/`, `/index` e `/listaClientes`.
