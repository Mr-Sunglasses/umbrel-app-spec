# umbrel-app-spec
umbrel-app-spec: enables validation and autocompletion for umbrel app packaging.

## configuration validation and auto-complete

In order to minimize friction and maximize productivity, Umbrel provides its own [schema.json](https://raw.githubusercontent.com/Mr-Sunglasses/umbrel-app-spec/refs/heads/master/umbrel-app.schema.json) for `umbrel-app.yml`. If your editor supports YAML schema validation, it's definitely recommended to set it up:

### Setup for [VS Code](https://code.visualstudio.com/)

1. Install [vscode-yaml](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml) for YAML language support.
2. Add the schema under the `yaml.schemas` key in your user or workspace [settings.json](https://code.visualstudio.com/docs/configure/settings) :

```
"yaml.schemas": {
    "https://raw.githubusercontent.com/Mr-Sunglasses/umbrel-app-spec/refs/heads/master/umbrel-app.schema.json": "umbrel-app.yml",
    "https://raw.githubusercontent.com/Mr-Sunglasses/umbrel-app-spec/refs/heads/master/docker-compose.schema.json": "docker-compose*.yml"
 },
```
