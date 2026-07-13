---
api_key_in: []
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Bnsf Authentication
name_suffix: Authentication
oauth_flows: []
overview: BNSF secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BNSF
provider_slug: bnsf
scheme_count: 1
schemes:
- description: 'BNSF customer APIs require certificate-based mutual TLS using a client

    certificate (PEM) issued by an approved Certificate Authority.'
  name: MutualTLS
  sources:
  - openapi/bnsf-openapi.yml
  type: mutualTLS
slug: bnsf-authentication
source_filename: bnsf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bnsf-openapi.yml\nsummary:\n  types:\n  - mutualTLS\nschemes:\n- name: MutualTLS\n  type: mutualTLS\n  description: |-\n    BNSF customer APIs require certificate-based mutual TLS using a client\n    certificate (PEM) issued by an approved Certificate Authority.\n  sources:\n  - openapi/bnsf-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/authentication/bnsf-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Freight
- Railroad
- Shipping
- Trains
- Intermodal
- Logistics
---
