---
api_key_in: []
api_specs:
- filename: apicurio-admin-api-openapi.yml
  format: yaml
  label: Apicurio Admin API
  slug: apicurio-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-admin-api-openapi.yml
- filename: apicurio-ai-api-openapi.yml
  format: yaml
  label: Apicurio AI API
  slug: apicurio-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-ai-api-openapi.yml
- filename: apicurio-artifact-rules-api-openapi.yml
  format: yaml
  label: Apicurio Artifact rules API
  slug: apicurio-artifact-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-artifact-rules-api-openapi.yml
- filename: apicurio-artifact-type-api-openapi.yml
  format: yaml
  label: Apicurio Artifact Type API
  slug: apicurio-artifact-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-artifact-type-api-openapi.yml
- filename: apicurio-artifacts-api-openapi.yml
  format: yaml
  label: Apicurio Artifacts API
  slug: apicurio-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-artifacts-api-openapi.yml
- filename: apicurio-branches-api-openapi.yml
  format: yaml
  label: Apicurio Branches API
  slug: apicurio-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-branches-api-openapi.yml
- filename: apicurio-content-api-openapi.yml
  format: yaml
  label: Apicurio Content API
  slug: apicurio-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-content-api-openapi.yml
- filename: apicurio-contracts-api-openapi.yml
  format: yaml
  label: Apicurio Contracts API
  slug: apicurio-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-contracts-api-openapi.yml
- filename: apicurio-gitops-api-openapi.yml
  format: yaml
  label: Apicurio GitOps API
  slug: apicurio-gitops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-gitops-api-openapi.yml
- filename: apicurio-global-rules-api-openapi.yml
  format: yaml
  label: Apicurio Global rules API
  slug: apicurio-global-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-global-rules-api-openapi.yml
- filename: apicurio-group-rules-api-openapi.yml
  format: yaml
  label: Apicurio Group rules API
  slug: apicurio-group-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-group-rules-api-openapi.yml
- filename: apicurio-groups-api-openapi.yml
  format: yaml
  label: Apicurio Groups API
  slug: apicurio-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-groups-api-openapi.yml
- filename: apicurio-kafkasql-api-openapi.yml
  format: yaml
  label: Apicurio KafkaSQL API
  slug: apicurio-kafkasql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-kafkasql-api-openapi.yml
- filename: apicurio-metadata-api-openapi.yml
  format: yaml
  label: Apicurio Metadata API
  slug: apicurio-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-metadata-api-openapi.yml
- filename: apicurio-search-api-openapi.yml
  format: yaml
  label: Apicurio Search API
  slug: apicurio-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-search-api-openapi.yml
- filename: apicurio-snapshot-api-openapi.yml
  format: yaml
  label: Apicurio Snapshot API
  slug: apicurio-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-snapshot-api-openapi.yml
- filename: apicurio-system-api-openapi.yml
  format: yaml
  label: Apicurio System API
  slug: apicurio-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-system-api-openapi.yml
- filename: apicurio-users-api-openapi.yml
  format: yaml
  label: Apicurio Users API
  slug: apicurio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-users-api-openapi.yml
- filename: apicurio-versions-api-openapi.yml
  format: yaml
  label: Apicurio Versions API
  slug: apicurio-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-versions-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Apicurio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Apicurio secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Apicurio
provider_slug: apicurio
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/apicurio-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://example.com/realms/apicurio/protocol/openid-connect/token
  name: OAuth2
  sources:
  - openapi/apicurio-openapi.yml
  type: oauth2
slug: apicurio-authentication
source_filename: apicurio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apicurio-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/apicurio-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/realms/apicurio/protocol/openid-connect/token\n    scopes: 3\n  sources:\n  - openapi/apicurio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/authentication/apicurio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Apache License
- API Design
- API Registry
- Avro
- AsyncAPI
- Java
- Open Source
- OpenAPI
- Red Hat
- Schema Registry
---
