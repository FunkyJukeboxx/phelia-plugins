# phelia_jackett

Jackett connector plugin for Phelia. It exposes a Torznab-backed SearchProvider.

## Features
- Settings panel in Phelia Settings:
  - `base_url` (Torznab root, default: `http://jackett:9117/api/v2.0/indexers/all/results/torznab`)
  - `api_key` (reads from `ServerConfig.json` if available)
  - `use_all_indexers` (reserved for future)
- Auto-detects Jackett on post-install if possible.
- Registers a SearchProvider on enable.

## Build
```bash
python -m pip install --upgrade build
python -m build
# dist/phelia_jackett-0.1.0-py3-none-any.whl

