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

## Design Guide

### Pokemon Theme Aesthetics

The app features a vibrant Pokemon-themed design with distinctive colors, playful typography, and Pokemon-inspired interactions. Maintain this cohesive aesthetic in all UI changes.

**Color Palette:**
- Primary: Pokemon Blue (#3B4CCA)
- Secondary: Pokemon Red (#FF0000)
- Accent: Pokemon Yellow (#FFDE00)
- Success: Pokemon Green (#78C850)
- Type Colors: Fire (#FF4422), Water (#3399FF), Grass (#77CC55), Electric (#FFCC33), Psychic (#FF5599), Dark (#664433)

**Typography:**
- Font: 'Fredoka One' for playful, rounded feel
- Hierarchy: Use text utilities for consistent sizing (text-xs to text-5xl)
- Emphasis: font-semibold/bold for key elements

**Visual Elements:**
- Background: Pokemon world gradient (sky to grass)
- Icons: Use Pokemon emojis (⚾, 🐭, ⚡) and symbols
- Animations: Pokeball shake for interactions, evolution effects for wins
- Borders: Rounded corners, Pokemon yellow borders for emphasis

### Frontend Design Principles

Avoid generic AI aesthetics by committing to distinctive, creative choices:

- **Typography**: Choose unique fonts like Fredoka One over generic options (Inter, Arial)
- **Color**: Dominant colors with sharp accents; avoid timid, evenly-distributed palettes
- **Motion**: Use CSS animations for high-impact moments (modal wins, square marking)
- **Backgrounds**: Layer gradients and effects for atmosphere rather than solid colors
- **Composition**: Unexpected layouts that feel genuinely designed for the Pokemon context

**Implementation Notes:**
- Use custom CSS utilities in `wwwroot/css/app.css`
- Components handle rendering only; logic stays in services
- Maintain responsive design and accessibility
- Test animations for smooth performance

---

## Style Guide

- **C#**: PascalCase for public members, follow `BingoGameService` conventions
- **CSS**: Use custom utility classes defined in `wwwroot/css/app.css`
- **Components**: Keep logic in services; components handle rendering only
- **Frontend Design**: See [frontend-design.instructions.md](.github/instructions/frontend-design.instructions.md) for distinctive, polished UI patterns

