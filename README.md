# Moneko – Smart Expense & Loan Tracker

**Moneko** is a personal finance mobile app designed to help you manage your spending, track loans, and gain insights into your financial behavior. Built with Kotlin, Jetpack Compose, Room DB, and modern Android development practices, Moneko is offline-first, intuitive, and delightful to use.

---

## 🚀 Features

- 📊 Track income and expenses with categories
- 💸 Record and manage borrowed/lent money with due dates
- 🧾 View your total balance and recent transactions at a glance
- 📈 Analyze spending via interactive pie and bar charts
- 🔄 Organized UI with bottom navigation
- 💡 Clean MVVM architecture with Hilt-based dependency injection
- 📦 Local-first data using Room (SQLite)

---

## 📐 Architecture Overview

Moneko follows **Clean Architecture** and **MVVM** pattern, separating responsibilities across layers for maintainability and scalability.

```plaintext
UI (Jetpack Compose)
  ↑
ViewModel (StateFlow + Logic)
  ↑
UseCases (Business Logic)
  ↑
Repository (Abstraction)
  ↑
Room DB (Persistence)

## Built With
| Tech/Library       | Purpose                   |
| ------------------ | ------------------------- |
| Kotlin             | Primary language          |
| Jetpack Compose    | UI Toolkit                |
| Room               | Local database            |
| Hilt               | Dependency Injection      |
| StateFlow          | Reactive state management |
| Navigation Compose | Multi-screen navigation   |

📱 Screens Overview
- Dashboard: Total balance, loan summary, recent transactions
= Transactions: View/add income or expenses
= Loans: View/add/manage borrowed or lent money
= Analysis: Pie chart by category, bar chart by month