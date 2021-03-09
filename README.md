# .Net-and-React-Tutorial
A project following the udemy tutorial "The complete guide to building an app from start to finish using ASP.NET Core, React (with Typescript) and Mobx"

TryCatchLearn resources for the reactivities project: https://github.com/TryCatchLearn/Reactivities

## Dotnet
- `dotnet -h` to see available commands.
- `dotnet watch run` run a project that is watched.
- `dotnet tool install --global dotnet-ef --version 5.0.3` globally installed ef.
- `dotnet ef migrations add Initial -p Persistence -s API` - how you create migrations!
- `dotnet new classlib -n Infrastructure` - add new project called Infrastructure.
- `dotnet sln add Infrastructure` - then add it to the solution.
- `dotnet add reference ../Application` - to add a ref from application to Infrastructure. this is more or less a dependency.

## React
- `npx create-react-app client-app --use-npm --template typescript`
- We can use <Fragment> or <> to contain react JSX, these do not translate to divs in markup.


## Layers
persistence: Data access layer.

- Good for debugging components and state.
https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en

- Axios can make http requests for react
https://github.com/axios/axios

- Project uses "Clean Architecture Pattern"

## CQRS + Mediator
Command and Query Responsibility Segregation
https://docs.microsoft.com/en-us/azure/architecture/patterns/cqrs

Mediator: Handles accepting a request and returning a response.

- Tutotial 41 if cancellation token becomes relevant.
- Can use standard VSCode debugger for the ASP.Net application.

## JSON to TS
Wow so cool: http://json2ts.com/

- Also you can use generics on JS functions, never realised.

## Clean the DB
- `dotnet ef database drop -s API -p Persistence`

## Refresh Imports
- `dotnet restore`

## Remove migrations with ef (before commited).
- `dotnet ef migrations remove -p Persistence -s API`

Total Tutorials: 288
Up to: 217 (75.3%)

23-02 - 16 to 48 (32)
  