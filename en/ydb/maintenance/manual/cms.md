---
sourcePath: en/ydb/ydb-docs-core/en/core/maintenance/manual/cms.md
---
# Updating configurations via CMS

## Get the current settings

The following command will let you get the current settings for a cluster or tenant.

```
./kikimr -s <endpoint> admin console configs load --out-dir <config-folder>
```

```
./kikimr -s <endpoint> admin console configs load --out-dir <config-folder> --tenant <tenant-name>
```

## Update the settings

First, you need to pull the desired config as indicated above and then prepare a protobuf file with an update request.

```
Actions {
  AddConfigItem {
    ConfigItem {
      Cookie: "<cookie>"
      UsageScope {
        TenantAndNodeTypeFilter {
          Tenant: "<tenant-name>"
        }
      }
      Config {
          <config-name> {
              <full-config>
          }
      }
    }
  }
}
```

The UsageScope field is optional and is needed to use settings for a specific tenant.

```
./kikimr -s <endpoint> admin console configs update <protobuf-file>
```

