# Copilot Workspace Instructions

## ✅ Mandatory Development Checklist

Before committing changes:

```bash
# 1. List – Understand structure
ls -la SocOps/{Components,Services,Models,Data,Pages}

# 2. Build – Verify compilation
dotnet build SocOps/SocOps.csproj

# 3. Test – Validate functionality
# (No tests yet – consider this an enhancement opportunity)
```

---

## Project Overview

**Soc Ops** is a Social Bingo game built with Blazor WebAssembly (.NET 10). Players find people matching questions to mark squares and get 5 in a row.

### Architecture Summary

```
SocOps/
├── Components/        # Blazor UI components
├── Services/          # BingoGameService (state), BingoLogicService (logic)
├── Models/            # GameState, BingoSquareData, BingoLine
├── Data/              # Questions.cs (static question bank)
├── Pages/             # Home.razor (main entry point)
└── wwwroot/           # Static assets & CSS utilities
```

---

## Key Patterns

| Pattern | Implementation |
|---------|-----------------|
| **State Management** | `BingoGameService` (scoped); persists via JS interop to localStorage |
| **Data Flow** | Component parameters ← Service state → EventCallback events |
| **Immutability** | Business logic returns new lists (LINQ `.Select()`, `.ToList()`) |
| **Styling** | Custom CSS utilities in `wwwroot/css/app.css` (layout, spacing, colors) |
| **Component Disposal** | `IDisposable` pattern to unsubscribe from state change events |

---

## Quick Commands

```bash
dotnet build SocOps/SocOps.csproj      # Build
dotnet run --project SocOps            # Run dev server (port 5166)
```

---

## Style Guide

- **C#**: PascalCase for public members, follow `BingoGameService` conventions
- **CSS**: Use custom utility classes defined in `wwwroot/css/app.css`
- **Components**: Keep logic in services; components handle rendering only
- **Frontend Design**: See [frontend-design.instructions.md](.github/instructions/frontend-design.instructions.md) for distinctive, polished UI patterns

