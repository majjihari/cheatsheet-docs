dotnet
======

To check dotnet version
-----------------------
dotnet --version

To create new solution "solution1"
----------------------------------
mkdir solution1
cd solution1
dotnet new sln

To create new project "project1" under "solution1"
--------------------------------------------------
Assume you are in solution1 directory.

mkdir project1
cd project1
dotnet new webapi --framework "net5.0"

To add project1 to solution1
----------------------------
assume you are in solution1\project1

dotnet sln ..\solution1.sln add project1.csproj

To build and run the project
----------------------------
Open project1 folder from vscode
*This will automatically install MSBuild tools and creates .vscode/launch.json and .vscode/tasks.json files.
