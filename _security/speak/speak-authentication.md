---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Speak Authentication
name_suffix: Authentication
oauth_flows: []
overview: Speak secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Speak
provider_slug: speak
scheme_count: 1
schemes:
- issuer: https://api.usespeak.com
  jwks_uri: https://api.usespeak.com/.well-known/jwks.json
  name: openIdConnect
  signing_algs:
  - RS256
  sources:
  - well-known/speak-openid-configuration.json
  token_endpoint: https://api.usespeak.com/v1/auth/token
  type: openIdConnect
slug: speak-authentication
source_filename: speak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.speak.com/.well-known/openid-configuration\ndocs: https://api.usespeak.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Derived from the provider's published OpenID Connect discovery document, not\n    from a public OpenAPI spec (Speak does not publish one). The Speak API is an\n    OAuth2/OIDC issuer serving the app clients; no scope reference, grant-type\n    list, or authorization endpoint is publicly documented, so flows are not\n    enumerated here.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  issuer: https://api.usespeak.com\n  token_endpoint: https://api.usespeak.com/v1/auth/token\n  jwks_uri: https://api.usespeak.com/.well-known/jwks.json\n  signing_algs:\n  - RS256\n  sources:\n  - well-known/speak-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speak/refs/heads/main/authentication/speak-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Ai
- Language Learning
- Education
- EdTech
- Speech
- Conversational AI
- Mobile
---
