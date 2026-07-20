---
api_key_in: []
api_specs:
- filename: hugging-face-transformers-openapi.json
  format: json
  label: Hugging Face Hub API
  slug: hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hugging-face-transformers/refs/heads/main/openapi/hugging-face-transformers-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hugging Face Transformers Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- tokenExchange
overview: Hugging Face Transformers secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and tokenExchange flow(s).
provider_name: Hugging Face Transformers
provider_slug: hugging-face-transformers
scheme_count: 2
schemes:
- description: 'User Access Token (hf_...) or OAuth access token (hf_oauth_...) passed as `Authorization: Bearer <token>`. User Access Tokens are created in account settings and can be fine-grained (scoped to repos/permissions) or classic (read / write / fine-grained). As of Jul 2026 tokens can be created from presets (Read-Only, Inference, Write, CI/CD, Full Access).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hugging-face-transformers-openapi.json
  type: http
- authorizationUrl: https://huggingface.co/oauth/authorize
  description: Sign in with Hugging Face — full OAuth 2.0 / OIDC authorization server. Authorization Code (PKCE S256), Device Code, and RFC 8693 Token Exchange (Enterprise) grants. See scopes/hugging-face-transformers-scopes.yml.
  deviceAuthorizationUrl: https://huggingface.co/oauth/device
  issuer: https://huggingface.co
  jwksUri: https://huggingface.co/oauth/jwks
  name: OAuth2
  sources:
  - https://huggingface.co/.well-known/openid-configuration
  tokenUrl: https://huggingface.co/oauth/token
  type: oauth2
  userinfoUrl: https://huggingface.co/oauth/userinfo
slug: hugging-face-transformers-authentication
source_filename: hugging-face-transformers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/hugging-face-transformers-openapi.json\ndocs: https://huggingface.co/docs/hub/security-tokens\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - deviceCode\n  - tokenExchange\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    User Access Token (hf_...) or OAuth access token (hf_oauth_...) passed as\n    `Authorization: Bearer <token>`. User Access Tokens are created in account\n    settings and can be fine-grained (scoped to repos/permissions) or classic\n    (read / write / fine-grained). As of Jul 2026 tokens can be created from\n    presets (Read-Only, Inference, Write, CI/CD, Full Access).\n  sources:\n  - openapi/hugging-face-transformers-openapi.json\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Sign in with Hugging Face — full OAuth 2.0 / OIDC authorization server.\n    Authorization Code (PKCE S256), Device Code, and RFC 8693 Token\
  \ Exchange\n    (Enterprise) grants. See scopes/hugging-face-transformers-scopes.yml.\n  issuer: https://huggingface.co\n  authorizationUrl: https://huggingface.co/oauth/authorize\n  tokenUrl: https://huggingface.co/oauth/token\n  deviceAuthorizationUrl: https://huggingface.co/oauth/device\n  userinfoUrl: https://huggingface.co/oauth/userinfo\n  jwksUri: https://huggingface.co/oauth/jwks\n  sources:\n  - https://huggingface.co/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hugging-face-transformers/refs/heads/main/authentication/hugging-face-transformers-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Computer Vision
- Deep Learning
- Machine Learning
- Natural Language Processing
- Open Source
- Transformers
---
