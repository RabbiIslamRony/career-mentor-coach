# Career Mentor Coach

Career Mentor Coach is a WordPress block theme for career mentors, executive coaches, interview advisors, and business consultants. It is built for Full Site Editing and includes templates, template parts, block patterns, style variations, bundled fonts, and placeholder visual assets.

Official WordPress.org theme page: https://wordpress.org/themes/career-mentor-coach/

## Current Release

- WordPress.org version: `1.0.1`
- Required WordPress version: `6.9`
- Required PHP version: `7.4`
- Text domain: `career-mentor-coach`

## Repository Structure

- `style.css` - theme metadata and front-end styles.
- `theme.json` - block theme settings, presets, and design tokens.
- `templates/` - full-site editing templates.
- `parts/` - reusable template parts such as header and footer.
- `patterns/` - registered block patterns used by the theme.
- `styles/` - color and typography style variations.
- `assets/` - images, fonts, and JavaScript.
- `inc/` - PHP includes for theme setup and pattern registration.

## Local Development

1. Copy this folder into a local WordPress install under `wp-content/themes/career-mentor-coach`.
2. Activate the theme from `Appearance > Themes`.
3. Test templates, patterns, navigation, styles, and responsive behavior in the Site Editor.
4. Keep all user-facing strings translation-ready when editing PHP files.

## Releases

The repository includes a GitHub Actions workflow that builds a clean WordPress theme ZIP whenever a version tag is pushed.

Use this pattern for the next release:

```bash
git add .
git commit -m "Prepare release 1.0.2"
git tag -a v1.0.2 -m "Career Mentor Coach 1.0.2"
git push origin main v1.0.2
```

The release ZIP excludes development-only files using `.distignore`.

## Support

For public support, use the official WordPress.org support forum linked from the theme page:

https://wordpress.org/themes/career-mentor-coach/

For code contributions, see [CONTRIBUTING.md](CONTRIBUTING.md).
