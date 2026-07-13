---
api_key_in:
- header
api_specs:
- filename: amazon-neptune-management-openapi.yml
  format: yaml
  label: Amazon Neptune Management API
  slug: amazon-neptune-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-management-openapi.yml
- filename: amazon-neptune-data-openapi.yml
  format: yaml
  label: Amazon Neptune Data API
  slug: amazon-neptune-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-data-openapi.yml
- filename: amazon-neptune-gremlin-openapi.yml
  format: yaml
  label: Neptune Gremlin API
  slug: neptune-gremlin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-gremlin-openapi.yml
- filename: amazon-neptune-sparql-openapi.yml
  format: yaml
  label: Neptune SPARQL API
  slug: neptune-sparql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-sparql-openapi.yml
- filename: amazon-neptune-opencypher-openapi.yml
  format: yaml
  label: Neptune openCypher API
  slug: neptune-opencypher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-opencypher-openapi.yml
- filename: amazon-neptune-streams-openapi.yml
  format: yaml
  label: Neptune Streams API
  slug: neptune-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-streams-openapi.yml
- filename: amazon-neptune-loader-openapi.yml
  format: yaml
  label: Neptune Loader API
  slug: neptune-loader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-loader-openapi.yml
- filename: amazon-neptune-ml-openapi.yml
  format: yaml
  label: Neptune ML API
  slug: neptune-ml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-ml-openapi.yml
- filename: amazon-neptune-analytics-openapi.yml
  format: yaml
  label: Neptune Analytics API
  slug: neptune-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/openapi/amazon-neptune-analytics-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Neptune Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Neptune secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Neptune
provider_slug: amazon-neptune
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: aws_sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-neptune-analytics-openapi.yml
  - openapi/amazon-neptune-data-openapi.yml
  - openapi/amazon-neptune-gremlin-openapi.yml
  - openapi/amazon-neptune-loader-openapi.yml
  - openapi/amazon-neptune-management-openapi.yml
  - openapi/amazon-neptune-ml-openapi.yml
  - openapi/amazon-neptune-opencypher-openapi.yml
  - openapi/amazon-neptune-sparql-openapi.yml
  - openapi/amazon-neptune-streams-openapi.yml
  type: apiKey
slug: amazon-neptune-authentication
source_filename: amazon-neptune-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-neptune-analytics-openapi.yml, openapi/amazon-neptune-data-openapi.yml,\n  openapi/amazon-neptune-gremlin-openapi.yml, openapi/amazon-neptune-loader-openapi.yml, openapi/amazon-neptune-management-openapi.yml,\n  openapi/amazon-neptune-ml-openapi.yml, openapi/amazon-neptune-opencypher-openapi.yml, openapi/amazon-neptune-sparql-openapi.yml,\n  openapi/amazon-neptune-streams-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: aws_sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-neptune-analytics-openapi.yml\n  - openapi/amazon-neptune-data-openapi.yml\n  - openapi/amazon-neptune-gremlin-openapi.yml\n  - openapi/amazon-neptune-loader-openapi.yml\n  - openapi/amazon-neptune-management-openapi.yml\n  - openapi/amazon-neptune-ml-openapi.yml\n  - openapi/amazon-neptune-opencypher-openapi.yml\n\
  \  - openapi/amazon-neptune-sparql-openapi.yml\n  - openapi/amazon-neptune-streams-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/authentication/amazon-neptune-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
---
