---
api_key_in: []
api_specs:
- filename: lambda-labs-asyncapi.yml
  format: yaml
  label: Lambda Inference API
  slug: inference-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/asyncapi/lambda-labs-asyncapi.yml
- filename: lambda-labs-audit-events-api-openapi.yml
  format: yaml
  label: Lambda Audit Events API
  slug: lambda-labs-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-audit-events-api-openapi.yml
- filename: lambda-labs-fabric-api-openapi.yml
  format: yaml
  label: Lambda Fabric API
  slug: lambda-labs-fabric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-fabric-api-openapi.yml
- filename: lambda-labs-filesystems-api-openapi.yml
  format: yaml
  label: Lambda Filesystems API
  slug: lambda-labs-filesystems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-filesystems-api-openapi.yml
- filename: lambda-labs-firewalls-api-openapi.yml
  format: yaml
  label: Lambda Firewalls API
  slug: lambda-labs-firewalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-firewalls-api-openapi.yml
- filename: lambda-labs-images-api-openapi.yml
  format: yaml
  label: Lambda Images API
  slug: lambda-labs-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-images-api-openapi.yml
- filename: lambda-labs-instances-api-openapi.yml
  format: yaml
  label: Lambda Instances API
  slug: lambda-labs-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-instances-api-openapi.yml
- filename: lambda-labs-regions-api-openapi.yml
  format: yaml
  label: Lambda Regions API
  slug: lambda-labs-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-regions-api-openapi.yml
- filename: lambda-labs-ssh-keys-api-openapi.yml
  format: yaml
  label: Lambda SSH keys API
  slug: lambda-labs-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-ssh-keys-api-openapi.yml
- filename: lambda-labs-support-tickets-api-openapi.yml
  format: yaml
  label: Lambda Support Tickets API
  slug: lambda-labs-support-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-support-tickets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lambda Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lambda secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lambda
provider_slug: lambda-labs
scheme_count: 2
schemes:
- description: 'Basic HTTP authentication. Allowed headers:

    * `Authorization: Basic <base64 encoding of api_key>:`

    * `Authorization: Basic <api_key>`'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/lambda-labs-openapi.json
  type: http
- description: 'Bearer HTTP authentication. Allowed headers:

    * `Authorization: Bearer <api_key>`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lambda-labs-openapi.json
  type: http
slug: lambda-labs-authentication
source_filename: lambda-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lambda-labs-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Basic HTTP authentication. Allowed headers:\n    * `Authorization: Basic <base64 encoding of api_key>:`\n    * `Authorization: Basic <api_key>`\n  sources:\n  - openapi/lambda-labs-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer HTTP authentication. Allowed headers:\n    * `Authorization: Bearer <api_key>`\n  sources:\n  - openapi/lambda-labs-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/authentication/lambda-labs-authentication.yml
summary_line: http · 2 schemes
tags:
- AI
- Cloud
- Clusters
- Compute
- GPU
- Inference
- Machine Learning
---
