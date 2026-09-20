# Jetpack Compose Stock Tracker App

A modern Android stock tracker application built with Jetpack Compose[cite: 3], featuring network data fetching via Retrofit, local database caching with Room, dependency injection, and advanced state management.

---

## Features

* **Jetpack Compose UI:** Declarative, modern UI screens including portfolio views and stock detail screens[cite: 3].
* **Network Integration:** Fetches live financial and stock data using Retrofit and custom API services.
* **Local Persistence & Caching:** Utilizes Room Database (`StockDao`, `PortFolioEntity`) for reliable offline data management.
* **Dependency Injection:** Configured with Hilt (`ViewModelHilt`, `AppModule`) for scalable and testable module architectures.
* **MVVM Architecture:** Clean separation of concerns with dedicated ViewModels, Factories, and Repositories driving UI states.

---

## Tech Stack

* **Language:** Kotlin
* **UI Toolkit:** Jetpack Compose[cite: 3]
* **Architecture:** MVVM + Repository Pattern
* **Networking:** Retrofit / OkHttp
* **Local Storage:** Room Database
* **Dependency Injection:** Hilt / Dagger

---

## Project Structure

```text
app/src/main/java/com/example/compose_fetch_stock_retrofit_navigate_r/
│
├── ui/theme/              # App themes, colors, and typography
├── AppModule.kt           # Dependency injection modules
├── Constants.kt           # Global constants and endpoint configurations
├── MainActivity.kt        # Entry point activity
├── PortFolioEntity.kt     # Database entity representations
├── PortFolio.kt           # Core portfolio data model
├── PortFolioScreen.kt     # Main portfolio UI view
├── PortFolioViewModel.kt  # ViewModels for business and state logic
├── RetrofitInstance.kt    # Retrofit network configuration client
├── Stock.kt               # Stock data model
├── StockApiService.kt     # Retrofit API endpoints interface
├── StockApplication.kt    # Application subclass for global configurations
├── StockDao.kt            # Room database data access object
├── StockDetailScreen.kt   # Stock detail view interface
└── StockRepository.kt     # Single source of truth data repository
