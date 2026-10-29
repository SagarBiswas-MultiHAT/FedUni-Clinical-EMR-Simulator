# Contributing to the EMR Simulator

Thank you for your interest in improving the EMR Simulator project. We welcome contributions that enhance educational value, stability, and code quality.

## Code of Conduct

All contributors and participants are expected to adhere to our [Code of Conduct](CODE_OF_CONDUCT.md).

## Getting Started

1. Fork the repository and create your branch from `main`.
2. Ensure you have the .NET 8.0 SDK and SQL Server Express installed.
3. Verify that the project builds locally:
   ```powershell
   dotnet build EMRSimulationWebApp/EMRSimulationWebApp/EMRSimulationWebApp.sln
   ```
4. Test your changes locally before submitting a Pull Request.

## Architecture Guidelines

This solution follows Clean Architecture principles:
- **EMRSimulation.Domain**: Core models, DTOs, and domain rules. No external project dependencies.
- **EMRSimulation.Application**: Interfaces, business services, and workflow logic.
- **EMRSimulation.Infrastructure**: Data access, SQL Server repositories, and external system integrations.
- **EMRSimulationWebApp**: Presentation layer using ASP.NET Core MVC, Razor views, and client scripts.

Please respect layer separation:
- Do not reference Infrastructure from Domain or Application.
- Keep controllers thin by routing operations through service interfaces.
- Use parameterized queries or stored procedures to prevent SQL injection.

## Intellectual Property and Licensing Notice

By submitting a pull request, you confirm that:
- Your contribution is original work.
- You grant the maintainers full rights to license and distribute the contribution as part of this project.
- No third-party proprietary assets, non-permissive libraries, or copyrighted hospital materials are introduced without explicit authorization.

## Submitting Pull Requests

1. Provide a clear, descriptive title following conventional commit styles (e.g., `feat:`, `fix:`, `docs:`).
2. Reference any related issue numbers in the description.
3. Ensure no unnecessary files (temporary files, build artifacts, or credentials) are committed.

