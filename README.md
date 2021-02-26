# Inventory_API JWT
Inventory_API (MSSql JWT)

#### 1. Description API
```
Demo API REST creada con .NET COre 3.1 utilizando JWT y conectada con base de datos 
MS Sql Virtualizada sobre Fedora 32  y Virtualbox 6.1. Aplicación con fines educativos.
```

#### 2. Link a un demo con el proyecto desplegado: https://github.com/JoseMarin/Inventory_API_JWT

```
* Nombre de la App: [GIT] (https://github.com/)
```
#### 3. Lista con los pasos mínimos que se necesitan para clonar exitosamente el proyecto y echarlo a andar en local.

###### Install
```
IDE               Visual Studio 2019 Community Version
Core              C# 
Framework         NET Core 3.1
DataBase          Microsoft Sql Server 
Virtual           VirtualBox 6.1
SO                Fedora 32
```
###### Packages Nuget 
```
Install-Package Microsoft.VisualStudio.Web.CodeGeneration.Design  -Version 3.1.4
Install-Package Microsoft.EntityFrameworkCore.Tools               -Version 3.1.8
Install-Package Microsoft.EntityFrameworkCore.SqlServer           -Version 3.1.8
Install-Package System.IdentityModel.Tokens.Jwt                   -Version 5.6.0
Install-Package Microsoft.AspNetCore.Authentication.JwtBearer     -Version 3.1.8
```
###### Cadena de Conexión Base de datos 
```
"AllowedHosts": "*",
  "ConnectionStrings": {
    "NetflixDatabase": "Server=192.168.1.135;Database=Inventory;User ID=usuario;Password=password"
    }
```
###### Scaffold-DbContext 
```
Scaffold-DbContext “Server=192.168.1.135;Database=Inventory;User ID=remote;Password=remote” 
Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models

```
#### 4. URIs endpoints.
```
Products
GET      /api/Products
POST     /api/Products
GET      /api/Products/{id}
PUT      /api/Products/{id}
DELETE   /api/Products/{id}
GET      /api/Products/stock

Token
POST     /api/Token ----> { "Email": "InventoryAdmin@abc.com", "Password": "$admin@2017" }

```
#### 5. Screenshot /home
![image](https://user-images.githubusercontent.com/16636086/107164559-ea896c00-69af-11eb-97e7-71f7a87d9bad.png)

