---
api_key_in: []
api_specs:
- filename: number26-xs2a-openapi-original.yml
  format: yaml
  label: N26 XS2A (Berlin Group PSD2)
  slug: n26-xs2a-berlin-group-psd2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/number26/refs/heads/main/openapi/number26-xs2a-openapi-original.yml
auth_types:
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Number26 Xs2A Authentication
name_suffix: Authentication
oauth_flows: []
overview: Number26 secures its APIs with http and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Number26
provider_slug: number26
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/number26-xs2a-openapi-original.yml
  type: http
- description: eIDAS QWAC (Qualified Website Authentication Certificate) required at the transport layer; role-specific certificates for AIS and PIS, with concurrent certificate support for automatic renewal.
  name: eidas-qwac
  sources:
  - https://github.com/n26/psd2-tpp-docs
  type: mutualTLS
slug: number26-xs2a-authentication
source_filename: number26-xs2a-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/number26-xs2a-openapi-original.yml\ndocs: https://github.com/n26/psd2-tpp-docs\nsummary:\n  types: [http, mutualTLS]\n  http_schemes: [bearer]\n  notes: >-\n    N26's XS2A (Access to Account) interface follows the Berlin Group NextGenPSD2\n    1.3.6 standard under EU PSD2. Third-party providers (AISP/PISP/CBPII) must\n    present a valid eIDAS QWAC certificate (role-specific for AIS vs PIS) at the\n    TLS layer (mutual TLS), then obtain an OAuth2 bearer access token via the\n    dedicated interface's authorization step before calling the account/consent\n    endpoints. Account-data calls additionally carry a Consent-ID header bound to\n    a previously approved consent.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    sources: [openapi/number26-xs2a-openapi-original.yml]\n  - name: eidas-qwac\n    type: mutualTLS\n    description: >-\n      eIDAS QWAC (Qualified Website Authentication Certificate)\
  \ required at the\n      transport layer; role-specific certificates for AIS and PIS, with concurrent\n      certificate support for automatic renewal.\n    sources: [https://github.com/n26/psd2-tpp-docs]\nconsent_binding:\n  header: Consent-ID\n  description: >-\n    Account information endpoints require a Consent-ID header referencing a\n    consent resource created via POST /consents and approved by the PSU.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/number26/refs/heads/main/authentication/number26-xs2a-authentication.yml
summary_line: http/mutualTLS · 2 schemes
tags:
- Company
- Fintech
- Banking
- Neobank
- Mobile Banking
- Payments
- Europe
- Germany
---
