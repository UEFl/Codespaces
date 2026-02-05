# Repository Mirror Setup

This repository is set up to track the upstream template repository from GitHub Education Resources.

## Upstream Template Repository

**Repository**: [github-education-resources/codespaces-project-template-js](https://github.com/github-education-resources/codespaces-project-template-js)

This is the official JavaScript Portfolio Site template with GitHub Codespaces and Copilot from GitHub Education.

## How the Mirror is Configured

The upstream template repository has been added as a remote named `template`. This allows you to:
- Pull updates from the upstream template
- Compare your local changes with the template
- Merge upstream improvements into your fork

## Working with the Template Remote

### View remote configuration
```bash
git remote -v
```

### Fetch latest changes from template
```bash
git fetch template
```

### View available branches from template
```bash
git branch -r | grep template
```

### Compare with template main branch
```bash
git diff template/main
```

### Merge updates from template (if needed)
```bash
git merge template/main
```

## Repository Structure

Both repositories share the same structure:
- `/.devcontainer` - Codespaces configuration
- `/src` - React application source files
- `/__images__` - Images and assets
- `/translations` - Localized documentation
- Configuration files for ESLint, Prettier, and package management

## Keeping Your Fork Updated

To keep your fork synchronized with the latest template updates:

1. Fetch the latest changes from the template:
   ```bash
   git fetch template
   ```

2. Review the changes:
   ```bash
   git log HEAD..template/main --oneline
   ```

3. Merge if desired:
   ```bash
   git merge template/main
   ```

4. Push to your repository:
   ```bash
   git push origin main
   ```

## Notes

- The template repository is read-only from this fork
- Always review changes before merging to avoid overwriting your customizations
- Consider creating a backup branch before merging significant updates
