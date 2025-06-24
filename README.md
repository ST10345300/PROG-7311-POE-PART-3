# PROG-7311-POE-PART-3
AgriEnergyConnect

AgriEnergyConnect is a role-based web application built with ASP.NET Core MVC and Entity Framework Core. It connects farmers and agricultural employees through digital tools for product management, order tracking, learning, and task monitoring. This system was developed as part of the PROG7311 Portfolio of Evidence (POE).

--------------------------------------------------------------------------------

Features

Authentication
- Role-based login (Farmer and Employee)
- Secure registration with password hashing

Farmer Capabilities
- View available products
- Add new products (name, category, price, description, image)
- Manage personal cart
- Place and track orders
- Access learning tools

Employee Capabilities
- Monitor and post updates on tasks
- View dashboard with analytics
- Access learning materials

Profile Management
- Update email, username, and password
- Role-based dashboard navigation

Analytics
- Farmer and Employee dashboards display relevant statistics and pie charts (via Chart.js)

--------------------------------------------------------------------------------

Technologies Used

- ASP.NET Core MVC (.NET 6+)
- Entity Framework Core
- SQL Server (LocalDB)
- Bootstrap 5
- Chart.js
- Razor Views (cshtml)

--------------------------------------------------------------------------------

Folder Structure

agri_connect/
├── Controllers/
│   ├── AccountController.cs
│   ├── FarmerController.cs
│   ├── EmployeeController.cs
│   ├── ProductController.cs
│   ├── CartController.cs
│   └── OrderController.cs
│
├── Models/
│   ├── User.cs
│   ├── Product.cs
│   ├── CartItem.cs
│   ├── Order.cs
│   └── EmployeeUpdate.cs
│
├── Data/
│   ├── AppDbContext.cs
│   └── Repositories/
│       └── ProductRepository.cs
│
├── Views/
│   ├── Shared/
│   ├── Farmer/
│   ├── Employee/
│   ├── Product/
│   ├── Cart/
│   ├── Order/
│   └── Account/
│
├── wwwroot/
│   ├── css/
│   ├── js/
│   └── images/

--------------------------------------------------------------------------------

Running the Project Locally

1. Prerequisites
- Visual Studio 2022 or later
- .NET 6 SDK
- SQL Server (LocalDB or SQL Express)

2. Setup Steps

# Clone the repository
git clone https://github.com/yourusername/agri_connect.git
cd agri_connect

# Restore NuGet packages
dotnet restore

# Apply EF Core migrations
dotnet ef database update

# Run the project
dotnet run

--------------------------------------------------------------------------------

Sample Logins

Farmer:
- Email: farmer@example.com
- Password: Test@123
- Role: Farmer

Employee:
- Email: employee@example.com
- Password: Test@123
- Role: Employee

--------------------------------------------------------------------------------

Contributors

- Rubben Shisso
- Submitted for: PROG7311 – Programming 3A
- Institution: [vc]

--------------------------------------------------------------------------------

License

This project is for educational purposes only.
All rights reserved © 2025.
