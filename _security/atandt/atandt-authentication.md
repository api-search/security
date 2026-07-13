---
api_key_in: []
api_specs:
- filename: atandt-wireless-apis.yaml
  format: yaml
  label: AT&T Wireless APIs
  slug: att-wireless-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-wireless-apis.yaml
- filename: atandt-network-apis.yaml
  format: yaml
  label: AT&T 5G Network APIs
  slug: att-network-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-network-apis.yaml
- filename: atandt-enterprise-connectivity-apis.yaml
  format: yaml
  label: AT&T Enterprise Connectivity APIs
  slug: att-enterprise-connectivity-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-enterprise-connectivity-apis.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Atandt Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: AT&T secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: AT&T
provider_slug: atandt
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://devex-web.att.com/oauth/token
  name: oauth2
  sources:
  - openapi/atandt-enterprise-connectivity-apis.yaml
  - openapi/atandt-network-apis.yaml
  type: oauth2
slug: atandt-authentication
source_filename: atandt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atandt-enterprise-connectivity-apis.yaml, openapi/atandt-network-apis.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://devex-web.att.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/atandt-enterprise-connectivity-apis.yaml\n  - openapi/atandt-network-apis.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/authentication/atandt-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 100
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
---
