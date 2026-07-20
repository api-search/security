---
api_key_in:
- header
- env
auth_types:
- apiKey
- http
- browserLogin
description: ''
kind: authentication
layout: security
method: searched
name: Cogniac Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cogniac secures its APIs with apiKey, http, and browserLogin across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cogniac
provider_slug: cogniac
scheme_count: 4
schemes:
- description: Per-user API key. Supplied via the COG_API_KEY environment variable, the api_key= constructor argument to CogniacConnection, or produced/stored by `cogniac auth login`. Sent on the authenticated session to api.cogniac.io.
  in: header
  name: apiKey
  type: apiKey
- description: Username/password login via COG_USER / COG_PASS (or constructor args), exchanged for a session/API key.
  name: usernamePassword
  scheme: basic
  type: http
- description: '`cogniac auth login` opens the browser and authenticates via the existing Cogniac web session (password or SAML SSO), then stores a per-user API key for subsequent CLI/SDK use.'
  name: browserLogin
  type: interactive
- description: Enterprise SAML single sign-on is supported through the web session that `cogniac auth login` rides on.
  name: samlSSO
  type: openIdConnect
slug: cogniac-authentication
source_filename: cogniac-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/Cogniac/skills/blob/main/skills/cogniac/SKILL.md\ndocs: https://docs.cogniac.io/\napi_base: https://api.cogniac.io/\nnotes: >-\n  Derived from the official Cogniac SDK/CLI and the provider-published agent\n  skill (no OpenAPI is published for the Cogniac public API). The public API is\n  a multi-tenant REST API; nearly every call also requires a tenant selection.\nsummary:\n  types: [apiKey, http, browserLogin]\n  api_key_in: [header, env]\n  oauth2_flows: []\n  multi_tenant: true\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    description: >-\n      Per-user API key. Supplied via the COG_API_KEY environment variable, the\n      api_key= constructor argument to CogniacConnection, or produced/stored by\n      `cogniac auth login`. Sent on the authenticated session to api.cogniac.io.\n  - name: usernamePassword\n    type: http\n    scheme: basic\n    description: >-\n      Username/password\
  \ login via COG_USER / COG_PASS (or constructor args),\n      exchanged for a session/API key.\n  - name: browserLogin\n    type: interactive\n    description: >-\n      `cogniac auth login` opens the browser and authenticates via the existing\n      Cogniac web session (password or SAML SSO), then stores a per-user API key\n      for subsequent CLI/SDK use.\n  - name: samlSSO\n    type: openIdConnect\n    description: >-\n      Enterprise SAML single sign-on is supported through the web session that\n      `cogniac auth login` rides on.\ntenant_selection:\n  required: true\n  mechanisms: [COG_TENANT env, '--tenant <tenant_id> CLI flag', 'tenant_id= SDK arg']\n  note: >-\n    A user authorized for more than one tenant must set a tenant explicitly;\n    omitting it raises ClientError(400) Unauthorized. Exceptions: `cogniac auth`\n    and `cogniac tenants` do not need a tenant.\ncredential_precedence:\n  - explicit args\n  - COG_API_KEY\n  - stored login (cogniac auth login)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogniac/refs/heads/main/authentication/cogniac-authentication.yml
summary_line: apiKey/http/browserLogin · 4 schemes
tags:
- Company
- Computer Vision
- Artificial Intelligence
- Machine Learning
- Visual Inspection
- Defect Detection
- Edge AI
- Manufacturing
- Industrial IoT
- MLOps
---
