# CSharp13-Lock_TryEnterExit-ASPNETCore_APIContagem
Exemplo em .NET 9 + ASP.NET Core + C#13 de API REST de contagem de acessos e que faz uso dos métodos TryEnter e Exit da classe Lock (namespace System.Threading).

Para testes de carga utilizei o package loadtest: https://www.npmjs.com/package/loadtest

Exemplo (30 usuários simultâneos, 1200 requisições): 

```bash
loadtest -n 1200 -c 30 -k http://localhost:5251/contador
```

Documentação sobre a classe Lock: https://learn.microsoft.com/en-us/dotnet/api/system.threading.lock?view=net-9.0
