# InventoryService

1. Create a web API using VS Code: https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-5.0&tabs=visual-studio-code
2. Install EF Core using .Net Core CLI (dotnet add package Microsoft.EntityFrameworkCore.SqlServer): https://docs.microsoft.com/en-us/ef/core/get-started/overview/install#net-core-cli
3. Add folder Models which contains a Context (InventoryContext.cs) and an Entity class (Product.cs)
4. Using DbContext with Denpendence Injection: dotnet add package Microsoft.EntityFrameworkCore.SqlServer
5. Verify and correct ConnectionStrings in appsetting.json to match your sql server.

#Database
1. Create a database named: Inventory
2. Create a table named Product

CREATE TABLE Product (
	Id INT IDENTITY(1,1) NOT NULL,
	Name VARCHAR(250) NOT NULL,
	CONSTRAINT PK_Product_Id PRIMARY KEY (Id)
)
