# SmartHostel
[![CI](https://github.com/sajidkamaljoy/SmartHostel/actions/workflows/ci.yml/badge.svg)](https://github.com/sajidkamaljoy/SmartHostel/actions/workflows/ci.yml)

> **Note:** this project was originally developed under my earlier GitHub account, [sajid43677/SmartHostel](https://github.com/sajid43677/SmartHostel), and was moved to this account in October 2026.

A smart hostel management solution for hostel owners. A Windows Forms desktop app written in C# for the OOP2 course.

## Group members

- Shajid Kamal Joy: 20-43677-2
- Kazi Rubab Bashar: 20-43661-2
- Al Shakib E Elahi: 20-43665-2

## Features

- **Login and registration** with separate admin and manager windows.
- **Resident management:** add, update and delete residents, and view resident information.
- **Room management:** assign and update room types for residents.
- **Employee management:** add, update and delete hostel staff, looked up by NID.
- **Service access:** toggle per-resident services such as meal, laundry, gym and games.
- **Expense tracking:** manage service expenses and view a monthly expense summary.

## Tech stack

C#, Windows Forms (.NET Framework 4.7.2), SQL Server accessed through `System.Data.SqlClient` (data-access code lives in `DataAccess.cs`).

## Run it

1. Create a SQL Server database named `smartHostel` with tables such as `ResidentInfo`, `ResidentRoomInfo`, `WorkEmployee`, `ServiceAccess`, `ServiceExpense` and `ServiceNameExpense`. The SQL script is not included in this repo.
2. In `DataAccess.cs` (and `DataAccesss.cs`), update the connection string for your own SQL Server instance and credentials.
3. Open `SmartHostel.sln` in Visual Studio and press F5.

## Notes

- The connection string in the source belongs to the original dev machine. Do not reuse its credentials. Use your own, and prefer Windows authentication or configuration over hard-coded passwords.
