---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Seeq Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Seeq secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Seeq
provider_slug: seeq
scheme_count: 3
schemes:
- description: Access keys are the recommended programmatic credential. A user generates an access key + password in Seeq and supplies them via spy.login(access_key=..., password=...); they authenticate as that user without interactive login.
  in: header
  name: AccessKey
  sources:
  - https://python-docs.seeq.com/
  type: apiKey
- description: Interactive username/password login resolved against a named authentication directory (e.g. Seeq built-in directory, Windows Auth, or a configured identity provider).
  name: UsernamePassword
  scheme: basic
  sources:
  - https://python-docs.seeq.com/
  type: http
- description: OAuth 2.0 / SSO login is supported for single sign-on identity providers configured on the Seeq Server, used for browser-based and delegated authentication.
  flows:
  - flow: authorizationCode
  name: OAuth2
  sources:
  - https://python-docs.seeq.com/
  type: oauth2
slug: seeq-authentication
source_filename: seeq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://python-docs.seeq.com/\ndocs: https://python-docs.seeq.com/\nnote: >-\n  Seeq exposes a REST API served per-instance by Seeq Server (self-hosted or Seeq Cloud) at /api,\n  with an interactive Swagger surface on the running instance. No public, cross-tenant OpenAPI is\n  published, so this profile is derived from the SPy (Python) login documentation rather than a spec.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: AccessKey\n  type: apiKey\n  in: header\n  description: >-\n    Access keys are the recommended programmatic credential. A user generates an access key + password\n    in Seeq and supplies them via spy.login(access_key=..., password=...); they authenticate as that user\n    without interactive login.\n  sources: [https://python-docs.seeq.com/]\n- name: UsernamePassword\n  type: http\n  scheme: basic\n  description: >-\n    Interactive\
  \ username/password login resolved against a named authentication directory\n    (e.g. Seeq built-in directory, Windows Auth, or a configured identity provider).\n  sources: [https://python-docs.seeq.com/]\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 / SSO login is supported for single sign-on identity providers configured on the Seeq\n    Server, used for browser-based and delegated authentication.\n  flows:\n  - flow: authorizationCode\n  sources: [https://python-docs.seeq.com/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seeq/refs/heads/main/authentication/seeq-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Manufacturing
- Industrial Analytics
- Time Series
- Machine Learning
- Artificial Intelligence
- Process Manufacturing
- Data Analytics
---
