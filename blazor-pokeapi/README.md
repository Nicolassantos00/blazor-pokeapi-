# BlazorPokeApi

Aplicação **Blazor WebAssembly** (.NET) que consome a [PokéAPI](https://pokeapi.co/) e exibe os dados de um Pokémon a partir do nome digitado.

Atividade da disciplina **Desenvolvimento Web – Usabilidade, Dev. Web, Mobile e Jogos** (Anima Educação).

## Funcionalidades

- Campo para digitar o nome do Pokémon (ex.: `pikachu`, `ditto`).
- Consulta ao endpoint `https://pokeapi.co/api/v2/pokemon/{nome}`.
- Exibe **imagem**, **ID**, **nome**, **altura** (m) e **peso** (kg).
- A imagem é lida do campo `sprites.other.official-artwork.front_default` do JSON.
- Mensagem de erro quando o Pokémon não é encontrado ou não há conexão.

## Tecnologias

- C# / .NET
- Blazor WebAssembly
- `HttpClient` com `System.Net.Http.Json`

## Como executar

1. Instale o [.NET SDK](https://dotnet.microsoft.com/download).
2. Clone o repositório:
   ```bash
   git clone https://github.com/<seu-usuario>/blazor-pokeapi.git
   cd blazor-pokeapi
   ```
3. Execute:
   ```bash
   dotnet run
   ```
4. Abra o endereço exibido no terminal (ex.: `http://localhost:5000`).

## Estrutura principal

```
Models/Pokemon.cs   -> classes que representam o JSON da API
Pages/Home.razor    -> página de busca e exibição do Pokémon
```

## Autores

- Nicolas Augusto Albuquerque dos Santos
- Felipe Ribeiro Gomes

## Licença

Distribuído sob a licença MIT. Veja o arquivo `LICENSE`.
