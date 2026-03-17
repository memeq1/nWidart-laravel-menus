## Installation via VCS (Version Control System)

You can also install this package directly from this GitHub fork using Composer's VCS (Version Control System) feature. This is useful if you want to use a customized version of the package.

### Step 1: Add Repository to composer.json

Add the repository configuration to your `composer.json`:

```json
"repositories": [
    {
        "type": "vcs",
        "url": "https://github.com/memeq1/nWidart-laravel-menus"
    }
]
```

### Step 2: Install the Package

**Option 1: Install latest development version**
```bash
composer require memeq1/nwidart-laravel-menus:dev-master
```

**Option 2: Install a specific version tag (Recommended)**
```bash
composer require memeq1/nwidart-laravel-menus:v7.0.0
```

Replace `v7.0.0` with the actual version tag from the repository.

### Step 3: Publish Configuration (Optional)

```bash
php artisan vendor:publish --provider="Widart\\LaravelMenus\\MenuServiceProvider"
```

> **⚠️ Warning:** Using `dev-master` in production is not recommended. Always use specific version tags for stability.
