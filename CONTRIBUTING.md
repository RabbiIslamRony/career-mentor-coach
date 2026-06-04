# Contributing to Career Mentor Coach

Thanks for helping improve Career Mentor Coach. This project is a WordPress.org block theme, so contributions should preserve theme review compatibility, accessibility, translation readiness, and clean release packaging.

## Contribution Scope

Good contribution areas include:

- Bug fixes for templates, patterns, styles, and front-end behavior.
- Accessibility improvements for navigation, focus states, color contrast, and semantic markup.
- Responsive layout fixes across desktop, tablet, and mobile breakpoints.
- Translation-readiness fixes for PHP strings.
- Documentation improvements for setup, release, and support workflows.
- Small visual refinements that preserve the theme's existing direction.

Avoid changes that:

- Add external tracking, remote assets, or third-party services.
- Introduce bundled dependencies without a clear need and license review.
- Replace existing self-created or licensed bundled assets without documentation.
- Change public theme identity, slug, text domain, or WordPress.org metadata casually.

## Development Setup

1. Clone the repository into a local WordPress install:

```bash
cd wp-content/themes
git clone https://github.com/RabbiIslamRony/career-mentor-coach.git
```

2. Activate `Career Mentor Coach` in `Appearance > Themes`.
3. Test changes in the WordPress Site Editor and on the front end.
4. Confirm that templates, template parts, patterns, style variations, and navigation still work.

## Coding Guidelines

- Follow WordPress coding standards for PHP, CSS, and JavaScript.
- Keep the text domain as `career-mentor-coach`.
- Escape output in PHP when adding dynamic content.
- Keep front-end assets local and license-compatible.
- Do not commit generated ZIP files, local environment files, dependency folders, or editor metadata.
- Keep changes focused and avoid unrelated refactors.

## Testing Checklist

Before opening a pull request, test:

- Theme activates without PHP errors.
- Site Editor opens and saves templates correctly.
- Front page, archive, single, page, search, and 404 templates render.
- Header, footer, and navigation work at mobile and desktop widths.
- Block patterns insert without broken images or invalid blocks.
- Style variations load correctly.
- Keyboard focus states are visible.
- `style.css` version and `readme.txt` stable tag are updated for release changes.

## Release Checklist

For maintainers preparing a new release:

1. Update `Version` in `style.css`.
2. Update `Stable tag` and changelog in `readme.txt`.
3. Commit the release changes.
4. Create and push a version tag:

```bash
git tag -a v1.0.2 -m "Career Mentor Coach 1.0.2"
git push origin main v1.0.2
```

5. Confirm the GitHub Actions release ZIP is attached to the GitHub release.
6. Submit or sync the release to WordPress.org through the normal theme workflow.

## Pull Request Notes

When opening a pull request, include:

- What changed.
- Why the change is needed.
- Screenshots for visual changes.
- The WordPress and PHP versions used for testing.
- Any accessibility, translation, or licensing notes.
