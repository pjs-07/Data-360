# Data-360

Salesforce DX (SFDX) project for Data-360.

## Structure

```text
force-app/main/default/   Salesforce metadata (source format)
config/                   Scratch org definition
scripts/                  Local utility scripts
sfdx-project.json         Project configuration
```

## Prerequisites

- [Salesforce CLI](https://developer.salesforce.com/tools/salesforcecli) (`sf`)
- Access to the target Salesforce / Data Cloud org

## Common commands

```bash
# Authenticate to an org
sf org login web --alias data360

# Deploy local source to a default org
sf project deploy start --source-dir force-app

# Retrieve metadata into this project
sf project retrieve start --source-dir force-app

# Open the default org
sf org open
```

## Branches

| Branch | Purpose |
|--------|---------|
| `proddatacloud` | Production Data Cloud |
| `stagingdatacloud` | Staging |
| `dev1datacloud` | Dev 1 |
| `dev2datacloud` | Dev 2 |
