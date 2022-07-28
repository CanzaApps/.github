# About Canza Finance
Canza finance is building the world's largest non-institutional-based financial system. Canza is utilizing Web3.0 and decentralized finance (DeFi) along with a robust network of experienced local money market players to distribute financial data and transaction-based services to the masses.

## Canza Finance Coding Style Guide
This style guide will cover every aspect of our engineering cycle from naming repositories, files, folders to code layout and best practices to our git workflow.

### Style Guide Note
The goal of this style guide is to provide consistency all across our projects. Consistency will improve the quality of code we write, increase readability and make it esy for us to onboard new developers.

Some of these guide are perculiar to a particular language while others will cut across the entire engineering workflow. A lot of the guide if not all follows industry standard making it easy for new developers joining the team to adapt to these standards.


### Naming Repositories, Folders and Files
- Repositories should be all lowercase, a repository with a compound word should be separated by a dash i.e canza-finance.
- Folders within a repository also should be all lowercase, a folder with a compound word should be separated by an underscore i.e smart_contracts.
- Files should use camelCase convention i.e bakiVault.sol.

### General Code Layout
- Use 4 spaces i.e 1 tab per indentation level (For typescript/javascript projects with a formatter such as prettier, ensure it is set to 4 spaces rather than 2 spaces).
- Write only one statement per line.
- Write only one declaration per line.
- Ensure each source file is wrapped.
- **Functions** should use camelCase and should describe exactly what actions they perform i.e ``function() getUserData`` and not ``function() userData``.
- **Classes**, **Structs**, **Interfaces**, **Events**, **Contracts** should use PascalCase i.e ``struct UserData`` not ``struct userData``.
- **Variables** should follow camelCase.

For a more exhaustive standard guide, check out https://docs.soliditylang.org/en/v0.8.15/style-guide.html.

NB: For Typescript and Javascript projects, we encourage the use of prettier for style formatting.

## Git WorkFlow
- Always work in a branch named to describe what feature you are implementing and branches should be named similar to repositories i.e trading-fees.
- After working on a feature and updating a branch, create a pull request to merge into develop branch. Develop branch will merge the changes after testing that the code works correctly.
- Commit messages should always describe what changes were made to a code or what new features were added.
- Master/Main should only contain WORKING, PRODUCTION code and can ONLY BE UPDATED by develop branch after all aspects of the new changes has been reviewed properly.
