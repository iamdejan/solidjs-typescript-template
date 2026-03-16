# AGENTS.md

## Code Generation

Make sure you adhere to the guide on this file to generate the code.

### Rules of engagement

1. You're allowed to create functions, structs and impl blocks to generate the code.
2. With the exception of import statements and Cargo macros (allow and deny), explain the flow of the program using comments. Make sure that you write not only what the program is doing, but why. It will help me to judge your work.
3. You have to add JSDoc. The JSDoc should contain what is the function for (basically the description), a brief summary of the steps, and input and output parameters. If your function has the ability to throw error, please state it in the JSDoc as well.
4. You're not allowed to add `// @ts-ignore` and/or `// @ts-nocheck`.

## Code Validation

After generating the code, make sure you validate the code you generated.

### Steps to Validate

Run these commands in sequence:
1. `pnpm run lint`: ensure no linter errors.
2. `pnpm run lint:fix`: if there is any linter error, fix it with this command.
3. `pnpm run lint`: recheck again, maybe there are linter errors that need manual fix.
4. `pnpm run build`: build the code. This ensures that there are no build errors.

## Update Documentation

After the validation is finished, update the project tree structure and file descriptions in README.md if needed. This is to ensure we always have updated documentation.
