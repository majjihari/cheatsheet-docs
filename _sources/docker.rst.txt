Build docker images for asp.net core web api
============================================

To check dotnet version
-----------------------
.. code-block:: none 

   dotnet --version

To create new solution "solution1"
----------------------------------
.. code-block:: none

   mkdir solution1
   cd solution1
   dotnet new sln
 
To create new project "project1" under "solution1"
--------------------------------------------------
Assume you are in solution1 directory.

.. code-block:: none 

   mkdir project1
   cd project1
   dotnet new webapi --framework "net5.0"

To add project1 to solution1
----------------------------
assume you are in solution1\project1

.. code-block:: none

   dotnet sln ..\solution1.sln add project1.csproj

To build and run the project
----------------------------
Open project1 folder from vscode and press F5.

**This will automatically install MSBuild tools and creates .vscode/launch.json and .vscode/tasks.json files.**

Open browser and type in url https://localhost:5001

Open browser and type in url https://localhost:5001/swagger


