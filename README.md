# MyBudget — Assignment 2

A layered C# console application for recording expenses and tracking a monthly budget. Built with .NET 10.

## Features

- Add one-time and recurring expenses.
- View expenses and monthly totals by category.
- Set a monthly budget and check its status.
- Save and load expenses as JSON.

## Projects

- **MyBudget.Core** — expense records, validation, budget rules, and repository.
- **MyBudget.Data** — JSON file storage.
- **MyBudget.App** — console menu and dependency injection setup.
- **MyBudget.Tests** — xUnit tests and an in-memory test store.

## Build, test, and run

Run these commands from the folder containing `MyBudget.sln`:

```sh
dotnet build MyBudget.sln
dotnet test MyBudget.Tests/MyBudget.Tests.csproj
dotnet run --project MyBudget.App/MyBudget.App.csproj
```

The app saves its data to `expenses.json` in its output folder.
