## Description
Provide a concise overview of the changes in this pull request and the problems they solve.

## Type of Change
- [ ] Bug fix (non-breaking change which fixes an issue)
- [ ] New clinical module / feature (non-breaking change which adds functionality)
- [ ] Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [ ] Documentation update

## Related Issues
Closes #(issue_number)

## Clean Architecture Checklist
- [ ] Changes adhere to layer separation (Domain -> Application -> Infrastructure -> WebApp)
- [ ] No database access logic directly inside Controllers
- [ ] Solution compiles cleanly without warnings or errors
- [ ] Tested locally with SQL Server Express

## Security & Sensitive Data Checklist
- [ ] No real patient information or identifiable data included
- [ ] No connection strings, passwords, or cryptographic keys committed

