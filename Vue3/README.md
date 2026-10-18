# Advanced search (Vue 3) — EasyQuery on Vue 3

**Advanced search.** A full-page query builder: users pick the columns, combine any conditions they need, run the query and work with the result — sorting, paging and export.

Part of [EasyQuery samples for ASP.NET Core + Vue](../README.md).

## Tech stack

| | |
|---|---|
| Host | ASP.NET Core 6 |
| UI | Vue 3 |
| Language | C#, TypeScript |
| EasyQuery | 7.5.0 — `Korzh.EasyQuery.AspNetCore`, `Korzh.EasyQuery.EntityFrameworkCore.Relational`, `Korzh.EasyQuery.SqlServerGate`, `Korzh.EasyQuery.SqLiteGate`, `Korzh.EasyQuery.DataExport` |
| EasyData | 1.6.0 — `EasyData.Exporters.ClosedXML`, `EasyData.Exporters.PdfSharp` |
| EasyQuery.JS | `@easydata/core` 1.6.0, `@easydata/ui` 1.6.0, `@easyquery/core` 7.5.1, `@easyquery/ui` 7.5.1, `@easyquery/enterprise` 7.5.1 |
| Database | SQLite or SQL Server Express LocalDB |

## Prerequisites

* [.NET 6 SDK](https://dotnet.microsoft.com/download)
* [Node.js](https://nodejs.org/) (LTS)
* Visual Studio 2022 17.2 or later, VS Code or any other editor (optional)
* SQL Server Express LocalDB (installed with Visual Studio)

## Run it

### Visual Studio

1. Open `Samples.Vue.sln` from the repository root.
2. Set both `AdvancedSearch.Server` and `AdvancedSearch.Client` as startup projects (Solution → Configure Startup Projects → Multiple startup projects).
3. Press F5.

### Command line

```bash
cd Vue3/AdvancedSearch.Server
dotnet run
```

The client is a separate project. In a second terminal:

```bash
cd Vue3/AdvancedSearch.Client
npm install
npm run dev
```

Then open the URL printed in the console.

## License key

EasyQuery needs a license key. Get a free 30-day trial key on
[korzh.com](https://korzh.com/easyquery?utm_source=github&utm_medium=sample&utm_campaign=eq-samples-aspnetcore-vue&utm_content=Vue3#get-started).

Put it into `appsettings.json` of the app that serves the EasyQuery API:

```json
"EasyQuery": {
  "LicenseKey": "your trial key goes here"
}
```

## Sample database

The demo database is created and filled automatically on the first start (about a minute or
two). It uses SQLite or SQL Server Express LocalDB; the connection string is in the app's configuration file.

## Related samples

* [Advanced search — ASP.NET Core Razor Pages and MVC](https://github.com/easyquery/eq-samples-aspnetcore-razor-mvc/tree/main/Razor.AdvancedSearch)
* [Advanced search — ASP.NET Core + Angular](https://github.com/easyquery/eq-samples-aspnetcore-angular/tree/main/AdvancedSearch)
* [Advanced search (Blazor Server) — ASP.NET Core + Blazor](https://github.com/easyquery/eq-samples-aspnetcore-blazor/tree/main/AdvancedSearch.BlazorServer)
* [Advanced search — ASP.NET Core + React](https://github.com/easyquery/eq-samples-aspnetcore-react/tree/main/AdvancedSearch)
* [Advanced search (Vue 2) — ASP.NET Core + Vue](https://github.com/easyquery/eq-samples-aspnetcore-vue/tree/main/Vue2)
* [Advanced search — ASP.NET Core + Stencil](https://github.com/easyquery/eq-samples-aspnetcore-stencil/tree/main/AdvancedSearch)
* [Advanced search — ASP.NET MVC 5 (.NET Framework)](https://github.com/easyquery/eq-samples-aspnet4-mvc/tree/main/AdvancedSearch)
* [Advanced search (separate front-end and service apps) — ASP.NET MVC 5 (.NET Framework)](https://github.com/easyquery/eq-samples-aspnet4-mvc/tree/main/AdvancedSearch-Multilayered)
* [Advanced search (C#) — ASP.NET Web Forms (.NET Framework)](https://github.com/easyquery/eq-samples-aspnet4-webforms/tree/main/AdvancedSearch)
* [Advanced search (Visual Basic) — ASP.NET Web Forms (.NET Framework)](https://github.com/easyquery/eq-samples-aspnet4-webforms/tree/main/VB.AdvancedSearch)
