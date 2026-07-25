---
api_key_in: []
api_specs:
- filename: dnsimple-accounts-api-openapi.yml
  format: yaml
  label: DNSimple Accounts API
  slug: dnsimple-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-accounts-api-openapi.yml
- filename: dnsimple-certificates-api-openapi.yml
  format: yaml
  label: DNSimple Certificates API
  slug: dnsimple-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-certificates-api-openapi.yml
- filename: dnsimple-contacts-api-openapi.yml
  format: yaml
  label: DNSimple Contacts API
  slug: dnsimple-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-contacts-api-openapi.yml
- filename: dnsimple-domains-api-openapi.yml
  format: yaml
  label: DNSimple Domains API
  slug: dnsimple-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-domains-api-openapi.yml
- filename: dnsimple-webhooks-api-openapi.yml
  format: yaml
  label: DNSimple Webhooks API
  slug: dnsimple-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-webhooks-api-openapi.yml
- filename: dnsimple-whoami-api-openapi.yml
  format: yaml
  label: DNSimple Whoami API
  slug: dnsimple-whoami-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-whoami-api-openapi.yml
- filename: dnsimple-zones-api-openapi.yml
  format: yaml
  label: DNSimple Zones API
  slug: dnsimple-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/openapi/dnsimple-zones-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dnsimple Authentication
name_suffix: Authentication
oauth_flows: []
overview: DNSimple secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DNSimple
provider_slug: dnsimple
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dnsimple-openapi.yml
  type: http
slug: dnsimple-authentication
source_filename: dnsimple-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dnsimple-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dnsimple-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnsimple/refs/heads/main/authentication/dnsimple-authentication.yml
summary_line: http · 1 scheme
tags:
- DNS
- Domains
---
