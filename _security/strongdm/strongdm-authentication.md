---
api_key_in:
- signed-request
auth_types:
- apiKey
description: StrongDM Admin API authentication. The control-plane API is gRPC; requests are authenticated with an API access key plus secret key pair generated in the Admin UI, and each request is signed. There is no OAuth 2.0 / OpenID Connect authorization-server surface on the API — the SDKs handle key-based signing internally, so there is no scope model (scopes/ is intentionally absent).
kind: authentication
layout: security
method: searched
name: Strongdm Authentication
name_suffix: Authentication
oauth_flows: []
overview: StrongDM secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StrongDM
provider_slug: strongdm
scheme_count: 1
schemes:
- description: API access key + secret key. The access key is a hex-format identifier (e.g. auth-0123abcd...); the secret is a paired string. Both are issued when an API key is created in the Admin UI and are supplied to the SDK via the SDM_API_ACCESS_KEY and SDM_API_SECRET_KEY environment variables. The SDK signs each gRPC request; the secret is never sent on the wire directly.
  env:
    access_key: SDM_API_ACCESS_KEY
    secret_key: SDM_API_SECRET_KEY
  in: header
  name: apiKeyPair
  sources:
  - docs.strongdm.com
  - github.com/strongdm/strongdm-sdk-python
  type: apiKey
slug: strongdm-authentication
source_filename: strongdm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.strongdm.com/ (API authentication) and the SDK READMEs\ndescription: >-\n  StrongDM Admin API authentication. The control-plane API is gRPC; requests are\n  authenticated with an API access key plus secret key pair generated in the\n  Admin UI, and each request is signed. There is no OAuth 2.0 / OpenID Connect\n  authorization-server surface on the API — the SDKs handle key-based signing\n  internally, so there is no scope model (scopes/ is intentionally absent).\nsummary:\n  types: [apiKey]\n  api_key_in: [signed-request]\n  oauth2_flows: []\nschemes:\n- name: apiKeyPair\n  type: apiKey\n  in: header\n  description: >-\n    API access key + secret key. The access key is a hex-format identifier\n    (e.g. auth-0123abcd...); the secret is a paired string. Both are issued when\n    an API key is created in the Admin UI and are supplied to the SDK via the\n    SDM_API_ACCESS_KEY and SDM_API_SECRET_KEY environment\
  \ variables. The SDK\n    signs each gRPC request; the secret is never sent on the wire directly.\n  env:\n    access_key: SDM_API_ACCESS_KEY\n    secret_key: SDM_API_SECRET_KEY\n  sources: [docs.strongdm.com, github.com/strongdm/strongdm-sdk-python]\nnotes: >-\n  Human access to resources is authenticated separately through the sdm client\n  and the organization's SSO/identity provider; this profile covers the Admin\n  API used for automation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strongdm/refs/heads/main/authentication/strongdm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Privileged Access Management
- Zero Trust
- Access Management
- Identity
- Infrastructure
- Audit
- Compliance
- DevOps
---
