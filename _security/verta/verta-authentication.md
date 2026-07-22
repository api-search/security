---
api_key_in: []
api_specs:
- filename: verta-APISync.swagger.json
  format: json
  label: Verta ModelDB REST API
  slug: verta-modeldb-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verta/refs/heads/main/openapi/verta-APISync.swagger.json
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
- Machine Learning
- Model Management
- Experiment Tracking
- Model Registry
- Model Versioning
- Metadata
- Open Source
- Company
---
