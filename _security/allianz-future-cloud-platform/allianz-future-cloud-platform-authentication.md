---
api_key_in: []
api_specs:
- filename: allianz-future-cloud-platform-services.yaml
  format: yaml
  label: Allianz Future Cloud Platform Services API
  slug: platform-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/openapi/allianz-future-cloud-platform-services.yaml
- filename: allianz-future-cloud-platform-policy.yaml
  format: yaml
  label: Allianz Insurance Policy Microservice API
  slug: policy-microservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/openapi/allianz-future-cloud-platform-policy.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Allianz Future Cloud Platform Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Allianz Future Cloud Platform secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
scheme_count: 1
schemes:
- description: OAuth2 for Allianz internal platform API access
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://platform.allianz.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/allianz-future-cloud-platform-services.yaml
  type: oauth2
slug: allianz-future-cloud-platform-authentication
source_filename: allianz-future-cloud-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-future-cloud-platform-services.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://platform.allianz.com/oauth2/token\n    scopes: 6\n  description: OAuth2 for Allianz internal platform API access\n  sources:\n  - openapi/allianz-future-cloud-platform-services.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/authentication/allianz-future-cloud-platform-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
---
