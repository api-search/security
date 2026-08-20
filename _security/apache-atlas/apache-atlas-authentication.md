---
api_key_in: []
api_specs:
- filename: apache-atlas-discovery-api-openapi.yml
  format: yaml
  label: Apache Atlas Discovery API
  slug: apache-atlas-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/openapi/apache-atlas-discovery-api-openapi.yml
- filename: apache-atlas-entities-api-openapi.yml
  format: yaml
  label: Apache Atlas Entities API
  slug: apache-atlas-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/openapi/apache-atlas-entities-api-openapi.yml
- filename: apache-atlas-glossary-api-openapi.yml
  format: yaml
  label: Apache Atlas Glossary API
  slug: apache-atlas-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/openapi/apache-atlas-glossary-api-openapi.yml
- filename: apache-atlas-lineage-api-openapi.yml
  format: yaml
  label: Apache Atlas Lineage API
  slug: apache-atlas-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/openapi/apache-atlas-lineage-api-openapi.yml
- filename: apache-atlas-relationships-api-openapi.yml
  format: yaml
  label: Apache Atlas Relationships API
  slug: apache-atlas-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/openapi/apache-atlas-relationships-api-openapi.yml
- filename: apache-atlas-types-api-openapi.yml
  format: yaml
  label: Apache Atlas Types API
  slug: apache-atlas-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/openapi/apache-atlas-types-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Atlas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Atlas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Atlas
provider_slug: apache-atlas
scheme_count: 1
schemes:
- description: HTTP Basic authentication with Atlas admin credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-atlas-rest-openapi.yaml
  type: http
slug: apache-atlas-authentication
source_filename: apache-atlas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-atlas-rest-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with Atlas admin credentials.\n  sources:\n  - openapi/apache-atlas-rest-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/authentication/apache-atlas-authentication.yml
summary_line: http · 1 scheme
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open-Source
---
