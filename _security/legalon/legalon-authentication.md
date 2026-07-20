---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Legalon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LegalOn secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LegalOn
provider_slug: legalon
scheme_count: 1
schemes:
- authorizationUrl: null
  flow: clientCredentials
  name: OAuth2ClientCredentials
  scopes: []
  scopes_published: false
  source: https://legalontech.jp/10843/
  tokenUrl: null
  type: oauth2
slug: legalon-authentication
source_filename: legalon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://legalontech.jp/10843/\ndocs: https://legalontech.jp/10843/\nnote: LegalOn publishes no open API reference. The authentication model below is taken\n  verbatim from LegalOn's own public API announcement; token and authorization\n  endpoint URLs are not published on the open web and are therefore not recorded here.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  authorizationUrl: null\n  tokenUrl: null\n  scopes: []\n  scopes_published: false\n  source: https://legalontech.jp/10843/\nauthorization:\n  model: workspace-scoped role-based access\n  description: API access is restricted to workspaces in which the authenticating\n    principal holds an appropriate role, as stated in the LegalOn API announcement.\ngaps:\n- No public authentication documentation page.\n- Token endpoint, authorization\
  \ server metadata, and scope names are not published.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration\n  document was found on any LegalOn host (see well-known/legalon-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legalon/refs/heads/main/authentication/legalon-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Technology
- Legal
- Legal Technology
- Contracts
- Contract Management
- Contract Lifecycle Management
- Artificial Intelligence
- Document Management
- Compliance
- Governance
- SaaS
- Japan
---
