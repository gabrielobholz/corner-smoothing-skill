# skills.sh Publishing Checklist

`skills.sh` installs skills from GitHub repositories using the open Agent Skills format.

## Publish Steps

1. Create a public GitHub repository, for example:

```text
gabrielobholz/corner-smoothing-skill
```

2. Push this folder to that repository.

3. Test installation:

```bash
npx skills add gabrielobholz/corner-smoothing-skill
```

4. If needed, install the exact skill path:

```bash
npx skills add gabrielobholz/corner-smoothing-skill/skills/gabrielobholz-corner-smoothing
```

5. The repository can then be linked from `skills.sh` and used by people who have the `skills` CLI available.

## Suggested Listing Text

Name:

```text
Corner Smoothing
```

Description:

```text
Apply Apple/iOS-style 60% corner smoothing to UI shapes with SVG paths, clip paths, Canvas Path2D, and radius-safe geometry instead of broken border-radius hacks.
```

Default prompt:

```text
Use $gabrielobholz-corner-smoothing to implement Apple/iOS-style 60% smoothed corners.
```

