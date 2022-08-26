# kawaii!!Wraps

kawaii!!Wraps Is an open source collection for boostrapping a large chunk of software dependencies for embedded use cases in Android!!

## Available Collections
- [waylovely](./waylovely) - Set of packages needed by a typical Wayland compositors on Android!!
- [xlovely](./xlovely) - Set of packages needded by a typical XWayland setup on Android!!
- [utils](./utils) - For libraries that are "utilities", they're not grouped for a certain setup, but packages might want to depend on individual packages!!

## How to use in Kawaii
You can add this to your `kawaii.toml` configuration!!

```toml
collections = [
    "https://github.com/waylovely-project/kawaii-wraps"
]
```

If you're adding a new package and want to depend on other packages, you can do that with:
```toml
deps = [
    "glib", "dbus", "libffi"
    # Add more as you wish!!
]
```
Say, you're making a Wayland compositor for Android, you can also do that!!
```toml
deps = ["waylovely/*"]
```