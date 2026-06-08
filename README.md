# Claim-mangement-system
A cloud-based digital platform designed to automate and streamline the end-to-end insurance and expense claims lifecycle. This system eliminates manual paperwork, accelerates approval workflows, and reduces processing errors through intelligent validation.

**Prerequisites
Ensure your system has the following components installed before starting:**
.NET SDK 8.0 (or your specific .NET Core version)
SQL Server (LocalDB or Express/Standard edition)
Visual Studio 2022 (or VS Code / .NET CLI)

** Installation & Setup
 Follow these steps exactly to extract, configure, and initialize the application database.**
 
 1. Extract the ProjectDownload the project .zip archive.Extract the contents to your preferred folder on your local machine.
 2. Configure the Database ConnectionOpen the project folder in Visual Studio or your preferred IDE.Locate and open the appsettings.json file in the root of the main project.
 3. Update the ConnectionStrings section with your local SQL Server details:

{
  "ConnectionStrings": {
    "DefaultConnection": "Server=YOUR_SERVER_NAME;Database=ClaimManagementDb;Trusted_Connection=True;MultipleActiveResultSets=true;TrustServerCertificate=True;"
  }
}

 **Run Database Migrations
 You must apply the migrations to generate the database schema and tables.
 Choose one of the methods below:
 Option A: **
 Using Visual Studio (Package Manager Console)Go to Tools > NuGet Package Manager > Package Manager Console.Ensure the Default Project is set to the project containing your Data Context.Run the following command:
 
 Update-Database

** Option B:**
 Using the .NET CLI (Terminal)Open your terminal or command prompt in the project root directory.
 Run the following command:

dotnet ef database update

**Running the Application
Once the database setup is complete, you can launch the system:**
In Visual Studio, click the green Start button (or press F5 / Ctrl + F5).
If using the CLI, run this command in your terminal:

dotnet run


