---
api_key_in: []
api_specs:
- filename: verta-authzservice-api-openapi.yml
  format: yaml
  label: Verta AuthzService API
  slug: verta-authzservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-authzservice-api-openapi.yml
- filename: verta-datasetservice-api-openapi.yml
  format: yaml
  label: Verta DatasetService API
  slug: verta-datasetservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-datasetservice-api-openapi.yml
- filename: verta-experimentrunservice-api-openapi.yml
  format: yaml
  label: Verta ExperimentRunService API
  slug: verta-experimentrunservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-experimentrunservice-api-openapi.yml
- filename: verta-experimentservice-api-openapi.yml
  format: yaml
  label: Verta ExperimentService API
  slug: verta-experimentservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-experimentservice-api-openapi.yml
- filename: verta-monitoredentityservice-api-openapi.yml
  format: yaml
  label: Verta MonitoredEntityService API
  slug: verta-monitoredentityservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-monitoredentityservice-api-openapi.yml
- filename: verta-projectservice-api-openapi.yml
  format: yaml
  label: Verta ProjectService API
  slug: verta-projectservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-projectservice-api-openapi.yml
- filename: verta-registryservice-api-openapi.yml
  format: yaml
  label: Verta RegistryService API
  slug: verta-registryservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-registryservice-api-openapi.yml
- filename: verta-scimconfigurationservice-api-openapi.yml
  format: yaml
  label: Verta SCIMConfigurationService API
  slug: verta-scimconfigurationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-scimconfigurationservice-api-openapi.yml
- filename: verta-stageservice-api-openapi.yml
  format: yaml
  label: Verta StageService API
  slug: verta-stageservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-stageservice-api-openapi.yml
- filename: verta-uacservice-api-openapi.yml
  format: yaml
  label: Verta UACService API
  slug: verta-uacservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-uacservice-api-openapi.yml
- filename: verta-versioningservice-api-openapi.yml
  format: yaml
  label: Verta VersioningService API
  slug: verta-versioningservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-versioningservice-api-openapi.yml
auth_types:
- custom
description: ''
kind: authentication
layout: security
method: searched
name: Verta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verta secures its APIs with custom across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Verta
provider_slug: verta
scheme_count: 0
schemes: []
slug: verta-authentication
source_filename: verta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.verta.ai/ + https://github.com/VertaAI/modeldb\nsummary:\n  types:\n  - custom\n  spec_declared: false\n  note: The harvested grpc-gateway REST specs declare no OpenAPI securityDefinitions.\nmodel:\n  scheme: Verta email + developer key\n  description: The hosted Verta platform authenticates the client against a backend host with a user email\n    and developer key; the open-source ModelDB quickstart connects to a host (e.g. http://localhost:3000)\n    and can run without credentials in local mode. Credentials are carried as gRPC metadata through the\n    grpc-gateway.\n  client_entrypoint: verta.Client(host, email=..., dev_key=...)\nscopes:\n  oauth2: false\n  note: No OAuth2 flows; authorization is enforced server-side via the UAC action/resource model, not\n    client-presented scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/authentication/verta-authentication.yml
summary_line: custom · 0 schemes
tags:
- MLOps
- Machine-Learning
- Model Management
- Experiment Tracking
- Model Registry
- Model Versioning
- Metadata
- Open-Source
- Company
---
