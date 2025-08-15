# 📚 Library App

## 📖 Description
**Library App** is a modular application designed to manage library operations such as book loans, patron management, and inventory tracking.  
It is built using **.NET** and follows a **Clean Architecture** approach to ensure scalability and maintainability.

---
## 🗂 Project Structure
```
LibraryApp/
│
├── AccelerateDevGHCopilot.sln         # Solution file for the project
│
├── src/                               # Main source code
│   ├── Library.ApplicationCore/       # Domain layer
│   │   ├── Entities/                  # Core domain entities
│   │   ├── Enums/                     # Enumerations used in the app
│   │   ├── Interfaces/                # Core abstraction interfaces
│   │   ├── Services/                  # Business logic and domain services
│   │   └── Library.ApplicationCore.csproj
│   │
│   ├── Library.Console/                # Console application
│   │   ├── appSettings.json            # Application settings
│   │   ├── CommonActions.cs            # Reusable console actions
│   │   ├── ConsoleApp.cs               # Main console logic
│   │   ├── ConsoleState.cs             # Console application state manager
│   │   ├── Json/                       # JSON utilities/data
│   │   ├── Program.cs                  # Entry point
│   │   └── Library.Console.csproj
│   │
│   ├── Library.Infrastructure/         # Infrastructure layer
│   │   ├── Data/                        # Data access implementations
│   │   └── Library.Infrastructure.csproj
│
└── tests/                               # Unit tests
    ├── UnitTests/
    │   ├── LoanFactory.cs               # Loan test data factory
    │   ├── PatronFactory.cs             # Patron test data factory
    │   ├── ApplicationCore/             # Domain layer unit tests
    │   └── UnitTests.csproj
```

---

## 🏗 Key Classes and Interfaces

### **Entities**
- `Book` — Represents a book in the library.
- `Patron` — Represents a library patron.
- `Loan` — Represents a loan transaction.

### **Interfaces**
- `IBookRepository` — Interface for book-related data operations.
- `IPatronRepository` — Interface for patron-related data operations.
- `ILoanService` — Interface for managing loan operations.

### **Services**
- `LoanService` — Implements loan-related business logic.
- `NotificationService` — Handles notifications for overdue loans.

---

## 🚀 Usage

1. **Clone the repository**
   ```bash
   git clone <repository-url>
2. **Clone the repository**
  ```bash
File: AccelerateDevGHCopilot.sln
  ```
3. **Build the solution**
 ```bash
dotnet build
```

4. **Run the console application**
```bash
dotnet run --project src/Library.Console/Library.Console.csproj
```
5. **Run unit tests**
```bash
dotnet test tests/UnitTests/UnitTests.csproj
```

---
## 📄 License
This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for more details.
