# Tests

!!! warning "Hinweis"
    noch nix

## 2. Überschrift

* a
* b
* c

### 3. Überschiftenlevel

```yaml
site_name: Handbuch für Game Entwicklung

theme:
  name: readthedocs

  highlightjs: true
  hljs_languages:
    - yaml
    - shell
    - json

markdown_extensions:
  - admonition
  - pymdownx.superfences:
      custom_fences:
        - name: mermaid
          class: mermaid
          format: !!python/name:pymdownx.superfences.fence_code_format
  - pymdownx.details

  - pymdownx.mark
  - pymdownx.tasklist:
      custom_checkbox: true
  - attr_list
  - pymdownx.highlight:
      use_pygments: true
      guess_lang: true
      linenums: true

plugins:
  - search:
      lang: de

extra_css:
  - https://unpkg.com/mermaid@8.8.0/dist/mermaid.css

extra_javascript:
  - https://unpkg.com/mermaid@8.8.0/dist/mermaid.min.js

nav:
  - Home: index.md
  - Tests: 
    - Generell: tests.md
    - Minecraft: minecraft.md
  - Blender: blender.md

``` 