---
anonymous_access: false
api_key_in: []
api_specs:
- filename: logius-announce-api-openapi.yml
  format: yaml
  label: Logius Announce API
  slug: logius-announce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-announce-api-openapi.yml
- filename: logius-contracts-api-openapi.yml
  format: yaml
  label: Logius Contracts API
  slug: logius-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-contracts-api-openapi.yml
- filename: logius-domains-api-openapi.yml
  format: yaml
  label: Logius Domains API
  slug: logius-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-domains-api-openapi.yml
- filename: logius-events-api-openapi.yml
  format: yaml
  label: Logius Events API
  slug: logius-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-events-api-openapi.yml
- filename: logius-manager-api-openapi.yml
  format: yaml
  label: Logius Manager API
  slug: logius-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-manager-api-openapi.yml
- filename: logius-peers-api-openapi.yml
  format: yaml
  label: Logius Peers API
  slug: logius-peers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-peers-api-openapi.yml
- filename: logius-services-api-openapi.yml
  format: yaml
  label: Logius Services API
  slug: logius-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-services-api-openapi.yml
- filename: logius-subscriptions-api-openapi.yml
  format: yaml
  label: Logius Subscriptions API
  slug: logius-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-subscriptions-api-openapi.yml
- filename: logius-terugmelding-api-openapi.yml
  format: yaml
  label: Logius Terugmelding API
  slug: logius-terugmelding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-terugmelding-api-openapi.yml
- filename: logius-terugmeldingstatus-api-openapi.yml
  format: yaml
  label: Logius Terugmelding Status API
  slug: logius-terugmeldingstatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-terugmeldingstatus-api-openapi.yml
- filename: logius-token-api-openapi.yml
  format: yaml
  label: Logius Token API
  slug: logius-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-token-api-openapi.yml
- filename: logius-well-known-api-openapi.yml
  format: yaml
  label: Logius .well Known API
  slug: logius-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-well-known-api-openapi.yml
auth_types:
- http
- mutualTLS
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Logius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Logius secures its APIs with http and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Logius
provider_slug: logius
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: JWT-Claims
  scheme: bearer
  sources:
  - openapi/logius-notificatieservices-openapi.yml
  type: http
- applies_to: FSC Core Manager API (logius:fsc-core-manager)
  description: Connections between Managers, Inways, Outways use Mutual Transport Layer Security (mTLS) with X.509 certificates. Participating Peers agree on a Root CA acting as Trust Anchor; the PeerID is determined by at least one element from the subject field of the X.509 certificate.
  name: FSC mTLS (X.509 / PKI trust anchor)
  note: Documented in the FSC Core standard (section 3.1 Identity and Trust); not declared as a securityScheme in the OpenAPI.
  sources:
  - https://logius-standaarden.github.io/fsc-core/
  type: mutualTLS
- applies_to: FSC Inway service calls; tokens issued by the Manager getToken operation (POST /token)
  description: Access tokens are carried in the HTTP header Fsc-Authorization; on a missing/invalid/expired token the WWW-Authenticate header MUST be set to Bearer.
  name: FSC access token (Fsc-Authorization header)
  scheme: bearer
  sources:
  - https://logius-standaarden.github.io/fsc-core/
  type: http
slug: logius-authentication
source_filename: logius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://logius-standaarden.github.io/fsc-core/\ndocs: https://logius-standaarden.github.io/fsc-core/\nsummary:\n  types:\n  - http\n  - mutualTLS\nschemes:\n- name: JWT-Claims\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/logius-notificatieservices-openapi.yml\n- name: FSC mTLS (X.509 / PKI trust anchor)\n  type: mutualTLS\n  applies_to: FSC Core Manager API (logius:fsc-core-manager)\n  description: \"Connections between Managers, Inways, Outways use Mutual Transport Layer Security (mTLS) with X.509 certificates. Participating Peers agree on a Root CA acting as Trust Anchor; the PeerID is determined by at least one element from the subject field of the X.509 certificate.\"\n  note: Documented in the FSC Core standard (section 3.1 Identity and Trust); not declared as a securityScheme in the OpenAPI.\n  sources:\n  - https://logius-standaarden.github.io/fsc-core/\n- name: FSC access token (Fsc-Authorization\
  \ header)\n  type: http\n  scheme: bearer\n  applies_to: FSC Inway service calls; tokens issued by the Manager getToken operation (POST /token)\n  description: \"Access tokens are carried in the HTTP header Fsc-Authorization; on a missing/invalid/expired token the WWW-Authenticate header MUST be set to Bearer.\"\n  sources:\n  - https://logius-standaarden.github.io/fsc-core/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/authentication/logius-authentication.yml
summary_line: http/mutualTLS · 3 schemes
tags:
- Company
- Government
- Netherlands
- API Standards
- API Design Rules
- Digital Identity
- Data Exchange
- Public Sector
---
