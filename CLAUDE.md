# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A static personal portfolio webpage for Rae Wilde. No build tools, frameworks, or dependencies — open `index.html` directly in a browser.

## Files

- `index.html` — markup and a small inline `<script>` for the dark/light mode toggle
- `styles.css` — all styling, linked from `index.html`

## Architecture Notes

**Theming** is driven by a `data-theme` attribute on `<html>`. CSS variables are defined in `:root` (light) and `[data-theme="dark"]` (dark). The toggle button in `index.html` sets this attribute and persists the preference to `localStorage`.

**Accent colour** is set via `--accent` and `--accent-light` in both theme blocks in `styles.css` — update both when changing the accent.
