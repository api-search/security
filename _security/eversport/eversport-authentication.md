---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Eversport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eversports secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eversports
provider_slug: eversport
scheme_count: 2
schemes:
- api: Eversports Provider API
  contact: support@eversports.com
  description: Provider-issued credentials required on every GraphQL request. Credentials are provisioned by Eversports (contact support@eversports.com) together with a Quick Start Guide; they scope the integration to the venues/companies that have activated the Provider API. Exact header name is provided with the credentials and is not publicly documented.
  in: header
  name: ProviderCredentials
  provisioning: https://helpcenter.eversportsmanager.com/what-is-the-provider-api
  sources:
  - https://helpcenter.eversportsmanager.com/what-is-the-provider-api
  type: apiKey
- api: Eversports Integration API (v2)
  description: The legacy JSON:API REST integration API (api.eversport.at/v2) is enabled by Eversports linking a partner/aggregator system to a venue via the venue UUID and company UUID (found under Settings > Aggregators in Eversports Manager). External systems then use client-side IDs and PUT for order upserts. No self-service API key is issued to the studio.
  name: AggregatorLinkage
  sources:
  - https://helpcenter.eversportsmanager.com/activate-the-workit-api
  - https://gist.github.com/thomasfr/e236f256a29f748b7956
  type: backend-linkage
slug: eversport-authentication
source_filename: eversport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://helpcenter.eversportsmanager.com/what-is-the-provider-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  notes: >-\n    Eversports does not publish an OpenAPI/GraphQL securityScheme document, so the\n    exact header name is not machine-derivable. Access to the GraphQL Provider API\n    is credential-gated: Eversports issues per-integration provider credentials on\n    request. The legacy JSON:API REST API is a partner/aggregator integration\n    activated via backend account linkage rather than self-service keys.\nschemes:\n- name: ProviderCredentials\n  api: Eversports Provider API\n  type: apiKey\n  in: header\n  description: >-\n    Provider-issued credentials required on every GraphQL request. Credentials\n    are provisioned by Eversports (contact support@eversports.com) together with a\n    Quick Start Guide; they scope the integration to the venues/companies that\n    have activated the Provider API.\
  \ Exact header name is provided with the\n    credentials and is not publicly documented.\n  provisioning: https://helpcenter.eversportsmanager.com/what-is-the-provider-api\n  contact: support@eversports.com\n  sources: [https://helpcenter.eversportsmanager.com/what-is-the-provider-api]\n- name: AggregatorLinkage\n  api: Eversports Integration API (v2)\n  type: backend-linkage\n  description: >-\n    The legacy JSON:API REST integration API (api.eversport.at/v2) is enabled by\n    Eversports linking a partner/aggregator system to a venue via the venue UUID\n    and company UUID (found under Settings > Aggregators in Eversports Manager).\n    External systems then use client-side IDs and PUT for order upserts. No\n    self-service API key is issued to the studio.\n  sources:\n  - https://helpcenter.eversportsmanager.com/activate-the-workit-api\n  - https://gist.github.com/thomasfr/e236f256a29f748b7956\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eversport/refs/heads/main/authentication/eversport-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Sports
- Fitness
- Booking
- Scheduling
- Wellness
- Marketplace
- GraphQL
- Reservations
- Studio Management
- Events
---
