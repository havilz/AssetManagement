<p align="center">
  <a href="https://dotnet.microsoft.com/en-us/apps/desktop" target="_blank">
    <img src="https://upload.wikimedia.org/wikipedia/commons/e/ee/.NET_Core_Logo.svg" alt=".NET 8 WPF" width="200">
  </a>
</p>

<p align="center">
    A modern, high-performance Asset Management System built with <strong>.NET 8</strong> and <strong>WPF</strong>.
</p>

<p align="center">
    <a href="#features">Features</a> •
    <a href="#getting-started">Getting Started</a> •
    <a href="#documentation">Documentation</a> •
    <a href="#technologies">Technologies</a> •
    <a href="#license">License</a>
</p>

---

## About The Project

The **Asset Management System** is a robust desktop application designed to streamline the tracking, management, and depreciation analysis of organizational assets. Built on the latest **.NET 8** framework and utilizing **Windows Presentation Foundation (WPF)**, it offers a visually stunning **Glassmorphism** user interface that is both beautiful and highly functional.

This project demonstrates a professional implementation of the **MVVM (Model-View-ViewModel)** architecture, ensuring a clean separation of concerns, testability, and maintainability.

## Features

### Asset Lifecycle Management

- **Complete CRUD Operations**: Create, read, update, and delete assets with a seamless user experience.
- **Real-Time Synchronization**: Updates are instantly reflected across all open views without manual refreshing.
- **Advanced Tracking**: Monitor assets by Code, Category, Location, Purchase Price, and Quantity.
- **Automated Depreciation**: Real-time calculation of current asset value using the Straight-Line depreciation method.

### Analytics & Reporting

- **Interactive Dashboard**: Visualize financial health with dynamic charts (Asset Value Growth, Category Distribution).
- **KPI Cards**: Instant visibility into Total Assets, Active Inventory, and Total Valuation.
- **Financial Reports**: Generate detailed depreciation reports in Excel (.xlsx) format for accounting purposes.

### Security & Access Control

- **Role-Based Access Control (RBAC)**: secure environment with Admin, Operator, and Viewer roles.
- **Granular Permissions**: Restrict access to sensitive features like User Management or Backup/Restore.
- **Secure Authentication**: Industry-standard SHA256 password hashing and secure session management.

### Data Integrity & Safety

- **Backup & Restore**: One-click database backup generation (.bak) and reliable restore functionality.
- **Import/Export**: Bulk data migration capabilities using Excel, complete with duplicate detection.
- **Audit Logging**: Comprehensive tracking of all critical system activities.

## Getting Started

### Prerequisites

- **.NET 8.0 SDK** or later.
- **SQL Server LocalDB** (included with Visual Studio).
- **Windows 10/11** operating system.

## 🔐 Default Login (Admin)

When running the application for the first time, use these credentials:

- **Username:** `admin`
- **Password:** `admin123`

> **Note:** After logging in, you can change the password or manage users in **Settings > Users**.

## 🛠️ Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/StartVision/AssetManagement.git
   ```

2. **Navigate to project directory**

   ```bash
   cd AssetManagement
   ```

3. **Restore dependencies**

   ```bash
   dotnet restore
   ```

4. **Run the application**
   ```bash
   dotnet run --project AssetManagement
   ```

The database will be automatically created and seeded with default data upon the first launch.

### Default Credentials

| Role              | Username | Password   | Access Level          |
| ----------------- | -------- | ---------- | --------------------- |
| **Administrator** | `admin`  | `admin123` | Full System Access    |
| **Operator**      |          |            | Asset Management Only |
| **Viewer**        |          |            | Read-Only Access      |

## Documentation

Comprehensive documentation is available in the `doc` directory:

- [Project Overview](doc/Project_Overview.md)
- [Architecture & Design](doc/Architecture.md)
- [Database Schema](doc/Database_Schema.md)
- [Setup Guide](doc/Setup_Guide.md)
- [Change Log](doc/Change_Log.md)

## Technologies

This project is built using a modern, robust technology stack:

- **Framework**: .NET 8.0 (Long Term Support)
- **UI Framework**: Windows Presentation Foundation (WPF)
- **Architecture**: Model-View-ViewModel (MVVM)
- **Database**: SQL Server LocalDB with Entity Framework Core 8
- **Charting**: LiveCharts (WPF)
- **File Processing**: ClosedXML (Excel)
- **Design System**: Custom Glassmorphism Theme

## License

This project is licensed for **Educational Use Only**.

- You may use, modify, and distribute this software for learning, teaching, and academic purposes.
- **Commercial use is strictly prohibited.**
- You may **NOT** sell, rent, or lease this software or any derivative works.

For more details, please see the [LICENSE](LICENSE) file.
