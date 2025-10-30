
---

### 2️⃣ Add This Code Inside the File
```yaml

name: Plugin Check

on:
  push:
    branches: [ "main" ]
  pull_request:
    branches: [ "main" ]

jobs:
  check:
    uses: CoolPluginsTeam/cool-plugins-ci/.github/workflows/plugin-check.yml@main
    with:
      plugin-folder: your-plugin-folder-name
