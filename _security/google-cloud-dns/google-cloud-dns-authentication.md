---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-cloud-dns-changes-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Changes API
  slug: google-cloud-dns-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-changes-api-openapi.yml
- filename: google-cloud-dns-policies-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Policies API
  slug: google-cloud-dns-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-policies-api-openapi.yml
- filename: google-cloud-dns-locations-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Cloud Dns Locations API
  slug: google-cloud-dns-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-locations-api-openapi.yml
- filename: google-cloud-dns-operations-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Cloud Dns Operations API
  slug: google-cloud-dns-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-operations-api-openapi.yml
- filename: google-cloud-dns-projects-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Cloud Dns Projects API
  slug: google-cloud-dns-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-projects-api-openapi.yml
- filename: google-cloud-dns-dnskeys-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Dns Keys API
  slug: google-cloud-dns-dnskeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-dnskeys-api-openapi.yml
- filename: google-cloud-dns-managedzoneoperations-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Managed Zone Operations API
  slug: google-cloud-dns-managedzoneoperations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-managedzoneoperations-api-openapi.yml
- filename: google-cloud-dns-managedzones-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Managed Zones API
  slug: google-cloud-dns-managedzones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-managedzones-api-openapi.yml
- filename: google-cloud-dns-outboundendpoints-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Outbound Endpoints API
  slug: google-cloud-dns-outboundendpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-outboundendpoints-api-openapi.yml
- filename: google-cloud-dns-responsepolicies-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Response Policies API
  slug: google-cloud-dns-responsepolicies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-responsepolicies-api-openapi.yml
- filename: google-cloud-dns-responsepolicyrules-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Response Policy Rules API
  slug: google-cloud-dns-responsepolicyrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-responsepolicyrules-api-openapi.yml
- filename: google-cloud-dns-resource-record-sets-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Resource Record Sets API
  slug: google-cloud-dns-resource-record-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-resource-record-sets-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Google Cloud DNS Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud DNS secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud DNS
provider_slug: google-cloud-dns
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/dns-openapi.yml
  type: oauth2
slug: google-cloud-dns-authentication
source_filename: google-cloud-dns-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dns-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/dns-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-dns/authentication/google-cloud-dns-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- DNS
- Domain Names
- Google Cloud
- Name Resolution
- Networking
---
