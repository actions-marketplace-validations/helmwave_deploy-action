# deploy-action

:octocat: GitHub Action for helmwave 

> This is archived. Please use https://github.com/helmwave/setup-action 

## Usage

*Workflow*

```yaml
name: helmwave

on:
  push:
    - master
    - main

jobs:
  helmwave:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: helmwave/deploy-action@1.0.0
        env:
          HELMWAVE_LOG_LVL: "debug"
```
