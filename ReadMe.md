
API->

<Nullable>enable</Nullable>
string? 

<ImplicitUsings>enable</ImplicitUsings>

Ctrl+p 




`dotnet --info`

`dotnet --help`

`mkdir reactivities`

`cd reactivities`

### Create solution in .net core

`dotnet new sln`


`dir`


### Create API in .net core

`dotnet new webapi -n API`

`dotnet new webapi -n API --dry-run`

`dotnet new webapi --use-controllers -o API`

`dotnet add package Microsoft.EntityFrameworkCore.InMemory`


`https://www.nuget.org/packages/Swashbuckle.AspNetCore`


### API.csproj file setup

```
<Project Sdk="Microsoft.NET.Sdk.Web">

  <PropertyGroup>
   <TargetFramework>net8.0</TargetFramework>
    <Nullable>enable</Nullable>
    <ImplicitUsings>enable</ImplicitUsings>
  </PropertyGroup>

  <ItemGroup>
    <PackageReference Include="Microsoft.AspNetCore.Diagnostics.EntityFrameworkCore" Version="8.0.0" />
    <PackageReference Include="Microsoft.AspNetCore.OpenApi" Version="8.0.0" />
    <!-- Other package references -->
    <PackageReference Include="Swashbuckle.AspNetCore" Version="6.4.0" />
  </ItemGroup>

</Project>

```

### build command

`dotnet build`

### 

`dotnet restore`


### run the API

`dotnet run`

`http://localhost:5050/swagger/index.html`



### Create Lib in .net core

`dotnet new classlib -n Application`


### Create lib with name Persistence

`dotnet new classlib -n Persistence`

`dir`

`dotnet sln`


### Add one or more projects to a solution file

`dotnet sln add API/API.csproj`

`dotnet sln add Application`


`dotnet sln add Persistence`

`dotnet sln add Domain`


### List all projects in a solution file

`dotnet sln list`


### 

cd API

`dotnet add reference ../Application`


cd Application


`dotnet add reference ../Persistence`

`dotnet add reference ../Domain`

cd ..

cd Persistence

`dotnet add reference ../Domain`









