---
api_key_in:
- header
api_specs:
- filename: rackspace-cloud-dns.yaml
  format: yaml
  label: Rackspace Cloud DNS API
  slug: cloud-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/openapi/rackspace-cloud-dns.yaml
- filename: rackspace-customer-service.yaml
  format: yaml
  label: Rackspace Customer Service API
  slug: customer-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/openapi/rackspace-customer-service.yaml
- filename: rackspace-cloud-identity.yaml
  format: yaml
  label: Rackspace Customer Identity API
  slug: customer-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/openapi/rackspace-cloud-identity.yaml
- filename: rackspace-offer.yaml
  format: yaml
  label: Rackspace Offer API
  slug: offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/openapi/rackspace-offer.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rackspace Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rackspace Technology secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rackspace Technology
provider_slug: rackspace-technology
scheme_count: 1
schemes:
- description: Rackspace Cloud Identity-issued authentication token.
  in: header
  name: AuthToken
  parameter: X-Auth-Token
  sources:
  - openapi/rackspace-cloud-dns.yaml
  - openapi/rackspace-cloud-identity.yaml
  - openapi/rackspace-customer-service.yaml
  - openapi/rackspace-offer.yaml
  type: apiKey
slug: rackspace-technology-authentication
source_filename: rackspace-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rackspace-cloud-dns.yaml, openapi/rackspace-cloud-identity.yaml, openapi/rackspace-customer-service.yaml,\n  openapi/rackspace-offer.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Rackspace Cloud Identity-issued authentication token.\n  sources:\n  - openapi/rackspace-cloud-dns.yaml\n  - openapi/rackspace-cloud-identity.yaml\n  - openapi/rackspace-customer-service.yaml\n  - openapi/rackspace-offer.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/authentication/rackspace-technology-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud
- Managed Services
- Multicloud
- Infrastructure
- DevOps
---
