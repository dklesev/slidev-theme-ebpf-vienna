# Contributing to slidev-theme-ebpf-vienna

Thank you for your interest in contributing to the eBPF Vienna Slidev theme! We welcome contributions from the community.

## Getting Started

1. Fork the repository
2. Clone your fork: `git clone https://github.com/YOUR_USERNAME/slidev-theme-ebpf-vienna.git`
3. Install dependencies: `pnpm install`
4. Start the development server: `pnpm run dev`

## Development Workflow

### Local Development

```bash
# Start dev server with example slides
pnpm run dev

# Build the example slides
pnpm run build

# Export to PDF
pnpm run export

# Generate PNG screenshots
pnpm run screenshot --output ./screenshots
```

### Making Changes

1. Create a new branch for your feature/fix: `git checkout -b feature/your-feature-name`
2. Make your changes in the appropriate files:
   - **Layouts**: `layouts/` directory
   - **Components**: `components/` directory
   - **Styles**: `styles/` directory
   - **Configuration**: `setup/` directory
3. Test your changes using the example slides in `example.md`
4. Commit your changes using [Conventional Commits](https://www.conventionalcommits.org/)

### Commit Message Format

We use Conventional Commits for automated versioning and changelog generation:

```
<type>(optional scope): <description>

[optional body]

[optional footer(s)]
```

Types:
- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that don't affect code meaning (formatting, etc.)
- `refactor`: Code change that neither fixes a bug nor adds a feature
- `perf`: Performance improvements
- `test`: Adding or updating tests
- `chore`: Changes to build process or auxiliary tools

Examples:
```
feat: add new layout for code-heavy slides
fix: correct logo positioning on cover layout
docs: update README with new layout examples
style: improve CSS organization and readability
```

## Code Style

- Use TypeScript for script sections in Vue components
- Follow Vue 3 Composition API best practices
- Use meaningful variable and function names
- Add comments for complex logic
- Keep CSS organized with clear sections

## Testing

Before submitting a pull request:

1. Ensure `pnpm run build` completes without errors
2. Test your changes with the example slides
3. Verify the theme works in both light and dark modes
4. Check that exports to PDF and PNG work correctly

## Pull Request Process

1. Update the `example.md` if you've added new features
2. Update documentation in `README.md` if needed
3. Push your changes to your fork
4. Create a Pull Request with a clear title and description
5. Link any relevant issues

## Release Process

Releases are automated using [release-please](https://github.com/googleapis/release-please):

- When PRs are merged to `main`, release-please creates/updates a release PR
- Merging the release PR triggers:
  - Version bump in `package.json`
  - CHANGELOG update
  - GitHub release creation
  - npm package publication

## Questions?

Feel free to open an issue for questions or discussions about contributing.

## Code of Conduct

Be respectful and inclusive. We're all here to learn and build something useful for the eBPF Vienna community.
