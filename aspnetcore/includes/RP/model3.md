<a name="cli"></a>
## <a name="add-scaffold-tooling-and-perform-initial-migration"></a>Adicionar ferramentas de scaffold e executar a migração inicial

Adicione as seguintes linhas ao arquivo *RazorPagesMovie.csproj*, logo antes da marca de fechamento `</Project>`:

```xml
<ItemGroup>
  <DotNetCliToolReference Include="Microsoft.VisualStudio.Web.CodeGeneration.Tools" Version="2.1.0-preview1-final"/>
</ItemGroup>
```  
Na linha de comando, execute os seguintes comandos de CLI do .NET Core:

```console
dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
dotnet restore
dotnet ef migrations add InitialCreate
dotnet ef database update
```

O elemento `DotNetCliToolReference` e o comando `add package` instalam as ferramentas necessárias para executar o mecanismo de scaffolding.

O comando `ef migrations add InitialCreate` gera código para criar o esquema de banco de dados inicial. O esquema é baseado no modelo especificado no `DbContext` (no arquivo *Models/MovieContext.cs*). O argumento `InitialCreate` é usado para nomear as migrações. Você pode usar qualquer nome, mas, por convenção, escolha um nome que descreve a migração. Consulte [Introdução às migrações](xref:data/ef-mvc/migrations#introduction-to-migrations) para obter mais informações.

O comando `ef database update` executa o método `Up` no arquivo *Migrations/\<time-stamp>_InitialCreate.cs*, que cria o banco de dados.
