# Corner Smoothing Skill

Apple/iOS-style 60% corner smoothing for AI coding agents.

This repository is compatible with [skills.sh](https://www.skills.sh) and the open Agent Skills format.

## Install

After this folder is published to GitHub, install it with:

```bash
npx skills add <owner>/<repo>
```

If the repository contains multiple skills, install this skill explicitly:

```bash
npx skills add <owner>/<repo>/skills/gabrielobholz-corner-smoothing
```

## Use

Ask your AI coding agent:

```text
Use $gabrielobholz-corner-smoothing to implement Apple/iOS-style 60% corner smoothing.
```

## What It Does

The skill teaches agents to implement Figma/Apple-style corner smoothing with path-based geometry instead of faking it with larger `border-radius` values.

It covers:

- SVG rounded rectangle paths
- CSS `clip-path: path(...)`
- Canvas `Path2D`
- Radius clamping
- `smoothing: 60` as the Apple/iOS-style default
- Layout-stable animation behavior

## Files

```text
skills/
  gabrielobholz-corner-smoothing/
    SKILL.md
    agents/openai.yaml
    references/implementation.md
```

## Plain Prompt Fallback

For AI platforms that do not support skills, use:

```text
Use Apple/iOS-style corner smoothing for UI shapes. Do not fake smoothing by increasing CSS border-radius. Use path-based geometry such as SVG path data, clip-path: path(...), Canvas Path2D, or equivalent vector paths. Use smoothing: 60 as the Apple/iOS/Figma-style default, clamp radius to min(width, height) / 2, preserve layout metrics, and animate the generated path rather than resizing the box.
```

