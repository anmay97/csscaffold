# csscaffold

A simple bash script that creates a basic CSS file structure for Rails applications.

**This is not a CSS framework.** It's just a scaffold - a starting point that gives you some structure and organization so you can write your own CSS.

## Installation

Copy the script to somewhere in your PATH:

```bash
cp csscaffold ~/.local/bin/
# or
sudo cp csscaffold /usr/local/bin/
```

## Usage

Run from the root of a Rails application:

```bash
csscaffold
```

The script will:
1. Verify you're in a Rails application directory
2. Show you the files it will create
3. Warn about any existing files (which will NOT be overwritten)
4. Ask for confirmation before proceeding

## Preview

Want to see what gets created before running it? Check out the [`examples/`](examples/) folder to see all 11 CSS files with their full content.

## Files Created

| File | Purpose |
|------|---------|
| `_global.css` | Global variables (spacing, text, borders, shadows, etc.) |
| `colors.css` | Color system and palette |
| `base.css` | Base element styles |
| `buttons.css` | Button styles |
| `dialog.css` | Modal/dialog styles |
| `flash.css` | Rails flash messages |
| `inputs.css` | Form inputs |
| `layout.css` | Page layout |
| `nav.css` | Navigation |
| `reset.css` | CSS reset |
| `utilities.css` | Utility classes |

## What You Get

- A `reset.css` with a modern CSS reset based on [Fizzy's reset](https://github.com/basecamp/fizzy/blob/main/app/assets/stylesheets/web/reset.css)
- A `colors.css` template showing how to organize your color system
- `@layer` declarations for CSS cascade control
- Commented-out examples following fizzy's patterns
- A sensible file organization to build on

The rest is up to you.

## Alternatives

**csscaffold** is intentionally minimal - it provides structure and a reset, but no pre-built components or utilities.

If you want something more comprehensive:

- **[css-zero](https://github.com/lazaronixon/css-zero)** - Pre-built CSS utilities and components for Rails, distributed as a gem. Good if you want a "no-build" CSS framework with conventions.

- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework. Good if you want extensive utilities and don't mind the build step.

- **[Pico CSS](https://picocss.com/)** - Classless CSS framework. Good if you want minimal pre-built styles for basic HTML elements.

- **[Water.css](https://watercss.dev/)** - Just add one `<link>` tag. Good if you want instant styling with zero setup.

**csscaffold is for you if:**
- You want structure without conventions
- You prefer writing your own CSS rather than using utilities
- You want a minimal reset and file organization to build on
