#  Fitness Club Management System

A comprehensive standalone desktop application developed in **C# Windows Forms (.NET)** for managing gym memberships, client data, and active subscriptions. Designed with an emphasis on user experience, robust data validation, and seamless deployment.

## Key Technical Features

* **Portable Database Architecture:** Integrates a local Microsoft SQL Server database (`SalaFitnessDB.mdf`). Custom dynamic connection strings utilizing `AppDomain.CurrentDomain.BaseDirectory` ensure the application runs out-of-the-box on any machine without complex SQL server configurations.
* **Relational Database Management:** Full CRUD operations built upon a normalized database schema connecting `Membri`, `Abonamente`, and `Inscrieri` through strict foreign key relationships.
* **Smart Data Visualization:** Implemented dynamic `DataGridView` rendering with automated row color-coding to instantly flag expired or expiring subscriptions, paired with advanced sorting and search filtering (e.g., querying by a 10-digit phone number).
* **Robust Input Validation:** Ensures data integrity through strict backend checks, validating Romanian phone number formats (exactly 10 digits) and logical subscription date intervals before allowing database commits.
* **Analytics & Statistics:** Built-in ADO.NET SQL queries to instantly generate and display active member statistics and subscription trends (Standard, Premium, VIP).

## Technology Stack
* **Language:** C#
* **Framework:** Windows Forms (.NET)
* **Database:** Microsoft SQL Server (LocalDB) & ADO.NET

## How to Run

1. Clone or download the repository.
2. Open the `.csproj` or `.sln` file in **Visual Studio**.
3. Ensure you have the `Data storage and processing` workload (SQL Server Express LocalDB) installed in Visual Studio.
4. Press `F5` to build and run. The database is localized and will attach automatically.
