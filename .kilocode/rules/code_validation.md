# Code Validation

Hi Kilo Code agent! Whatever model you are using, make sure you validate the code you generated.

## Steps to Validate

Run these commands in sequence:
1. `pnpm run lint`: ensure no linter errors.
2. `pnpm run lint:fix`: if there is any linter error, fix it with this command.
3. `pnpm run lint`: recheck again, maybe there are linter errors that need manual fix.
4. `pnpm run build`: build the code. This ensures that there are no build errors.
