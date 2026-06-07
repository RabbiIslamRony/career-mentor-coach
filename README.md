# Career Mentor Coach

Career Mentor Coach is a WordPress block theme for career mentors, executive coaches, interview advisors, and business consultants. It is built for Full Site Editing and includes templates, template parts, block patterns, style variations, bundled fonts, and placeholder visual assets.

Official WordPress.org theme page: https://wordpress.org/themes/career-mentor-coach/

## Current Release

- Repository release target: `1.0.2`
- Required WordPress version: `6.9`
- Tested up to WordPress: `7.0`
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
The workflow syncs the packaged theme version from the tag name, so a `vX.Y.Z` tag produces a ZIP with `Version: X.Y.Z` and `Stable tag: X.Y.Z`.

The GitHub release ZIP can be submitted manually to WordPress.org, or the approved version can be deployed through the WordPress.org SVN workflow once secure credentials are configured.

The WordPress.org release target is `1.0.2`. The GitHub `v1.0.2` tag has been replaced with the approved `main` release commit.

## WordPress.org SVN Deploy

After the theme is approved on WordPress.org, updates can be deployed to `https://themes.svn.wordpress.org/career-mentor-coach/` with the `Deploy WordPress.org theme SVN` workflow.

Required GitHub repository secrets:

- `SVN_USERNAME`: WordPress.org username with commit access to the theme.
- `SVN_PASSWORD`: WordPress.org password for that account.

For the current WordPress.org release target, run the workflow manually with version `1.0.2`. If WordPress.org import fails before publishing, the workflow can re-commit fixes to the same version directory. For future approved releases, merge the release commit to `main`, tag the version, and deploy the matching version directory to SVN.

Use this pattern for future confirmed releases:

```bash
git add .
git commit -m "Prepare release X.Y.Z"
git tag -a vX.Y.Z -m "Career Mentor Coach X.Y.Z"
git push origin main vX.Y.Z
```

Do not create or push the release tag until the maintainer confirms the release is ready.

The release ZIP excludes development-only files using `.distignore`.

## Support

For public support, use the official WordPress.org support forum linked from the theme page:

https://wordpress.org/themes/career-mentor-coach/

For code contributions, see [CONTRIBUTING.md](CONTRIBUTING.md).
