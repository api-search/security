---
api_key_in: []
api_specs:
- filename: anchore-images-api-openapi.yml
  format: yaml
  label: Anchore Images API
  slug: anchore-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-images-api-openapi.yml
- filename: anchore-policies-api-openapi.yml
  format: yaml
  label: Anchore Policies API
  slug: anchore-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-policies-api-openapi.yml
- filename: anchore-registries-api-openapi.yml
  format: yaml
  label: Anchore Registries API
  slug: anchore-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-registries-api-openapi.yml
- filename: anchore-sbom-api-openapi.yml
  format: yaml
  label: Anchore SBOM API
  slug: anchore-sbom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-sbom-api-openapi.yml
- filename: anchore-subscriptions-api-openapi.yml
  format: yaml
  label: Anchore Subscriptions API
  slug: anchore-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-subscriptions-api-openapi.yml
- filename: anchore-vulnerabilities-api-openapi.yml
  format: yaml
  label: Anchore Vulnerabilities API
  slug: anchore-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-vulnerabilities-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Anchore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anchore secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Anchore
provider_slug: anchore
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/anchore-enterprise-api.yaml
  type: http
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/anchore-enterprise-api.yaml
  type: http
slug: anchore-authentication
source_filename: anchore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anchore-enterprise-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/anchore-enterprise-api.yaml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/anchore-enterprise-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/authentication/anchore-authentication.yml
summary_line: http · 2 schemes
tags:
- Container Security
- Containers
- SBOM
- Software Supply Chain
- Vulnerability Scanning
---
