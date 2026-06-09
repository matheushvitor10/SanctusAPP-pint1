# Sanctus App — Food Truck Manager

# REQUISITOS

O computador precisa ter:

- .NET 10 SDK instalado
- MySQL Server instalado e rodando

Verificar .NET:

```bash
dotnet --version
```

Deve aparecer algo parecido com:

```txt
10.0.xxx
```

---

# 1. ABRIR O PROJETO

Abrir CMD ou PowerShell.

Entrar na pasta do projeto:

```bash
cd C:\Projetos\SanctusAppV2
```

ou no caminho onde o projeto estiver salvo.

---

# 2. RESTAURAR PACOTES NUGET

Executar:

```bash
dotnet restore
```

Isso baixa automaticamente todos os pacotes necessários do projeto.

---

# 3. CONFIGURAR O BANCO

Abrir:

```txt
appsettings.json
```

Editar:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=localhost;Port=3306;Database=sanctuspanis_db;User=root;Password=SUA_SENHA;"
}
```

Trocar:

```txt
SUA_SENHA
```

pela senha do MySQL.

---

# 4. CRIAR O BANCO DE DADOS

Abrir MySQL Workbench e executar:

```sql
CREATE DATABASE sanctuspanis_db;
```

---

# 5. RODAR O PROJETO

Executar:

```bash
dotnet run
```

---

# 6. ABRIR NO NAVEGADOR

O terminal mostrará algo parecido com:

```txt
Now listening on: http://localhost:5209
```

Abrir a URL no navegador.

Exemplo:

```txt
http://localhost:5209
```

---

# LOGIN PADRÃO

```txt
Email:
admin@sanctuspanis.com

Senha:
Admin@123
```

---

# COMANDOS IMPORTANTES

## Restaurar pacotes

```bash
dotnet restore
```

## Rodar projeto

```bash
dotnet run
```

## Build do projeto

```bash
dotnet build
```

## Limpar build

```bash
dotnet clean
```

---

# POSSÍVEIS ERROS

## Access denied for user 'root'@'localhost'

Verificar:
- senha do MySQL
- appsettings.json

---

## Porta já em uso

Editar:

```txt
Properties/launchSettings.json
```

---

## Projeto bloqueado pela faculdade

Mover o projeto para:

```txt
C:\Projetos
```

Evitar:
- Downloads
- Desktop

---
