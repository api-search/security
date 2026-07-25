---
api_key_in: []
api_specs:
- filename: mon-ami-care-plans-api-openapi.yml
  format: yaml
  label: Mon Ami Care Plans API
  slug: mon-ami-care-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-care-plans-api-openapi.yml
- filename: mon-ami-client-calls-api-openapi.yml
  format: yaml
  label: Mon Ami Client Calls API
  slug: mon-ami-client-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-client-calls-api-openapi.yml
- filename: mon-ami-clients-api-openapi.yml
  format: yaml
  label: Mon Ami Clients API
  slug: mon-ami-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-clients-api-openapi.yml
- filename: mon-ami-copays-api-openapi.yml
  format: yaml
  label: Mon Ami Copays API
  slug: mon-ami-copays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-copays-api-openapi.yml
- filename: mon-ami-documents-api-openapi.yml
  format: yaml
  label: Mon Ami Documents API
  slug: mon-ami-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-documents-api-openapi.yml
- filename: mon-ami-funding-sources-api-openapi.yml
  format: yaml
  label: Mon Ami Funding Sources API
  slug: mon-ami-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-funding-sources-api-openapi.yml
- filename: mon-ami-languages-api-openapi.yml
  format: yaml
  label: Mon Ami Languages API
  slug: mon-ami-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-languages-api-openapi.yml
- filename: mon-ami-people-api-openapi.yml
  format: yaml
  label: Mon Ami People API
  slug: mon-ami-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-people-api-openapi.yml
- filename: mon-ami-programs-api-openapi.yml
  format: yaml
  label: Mon Ami Programs API
  slug: mon-ami-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-programs-api-openapi.yml
- filename: mon-ami-provider-referrals-api-openapi.yml
  format: yaml
  label: Mon Ami Provider Referrals API
  slug: mon-ami-provider-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-provider-referrals-api-openapi.yml
- filename: mon-ami-providers-api-openapi.yml
  format: yaml
  label: Mon Ami Providers API
  slug: mon-ami-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-providers-api-openapi.yml
- filename: mon-ami-services-api-openapi.yml
  format: yaml
  label: Mon Ami Services API
  slug: mon-ami-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-services-api-openapi.yml
- filename: mon-ami-sites-api-openapi.yml
  format: yaml
  label: Mon Ami Sites API
  slug: mon-ami-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-sites-api-openapi.yml
- filename: mon-ami-tasks-api-openapi.yml
  format: yaml
  label: Mon Ami Tasks API
  slug: mon-ami-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-tasks-api-openapi.yml
- filename: mon-ami-visits-api-openapi.yml
  format: yaml
  label: Mon Ami Visits API
  slug: mon-ami-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-visits-api-openapi.yml
- filename: mon-ami-volunteers-api-openapi.yml
  format: yaml
  label: Mon Ami Volunteers API
  slug: mon-ami-volunteers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-volunteers-api-openapi.yml
- filename: mon-ami-webhooks-api-openapi.yml
  format: yaml
  label: Mon Ami Webhooks API
  slug: mon-ami-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mon Ami Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mon Ami secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mon Ami
provider_slug: mon-ami
scheme_count: 1
schemes:
- credential: uid:secret
  location: Authorization header
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mon-ami-openapi.yml
  type: http
slug: mon-ami-authentication
source_filename: mon-ami-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.monami.io/\ndocs: https://docs.monami.io/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Mon Ami uses HTTP Basic authentication. Credentials are a uid and secret pair\n  passed in the Authorization header as \"Basic base64(uid:secret)\". API credentials\n  are provisioned by Mon Ami (contact the team via the docs to obtain access).\n  No OAuth 2.0 or API-key-header scheme is documented.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    credential: uid:secret\n    location: Authorization header\n    sources: [openapi/mon-ami-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/authentication/mon-ami-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Aging Services
- Disability Services
- Case Management
- Care Coordination
- HL7 FHIR
- HIPAA
---
