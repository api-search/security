---
api_key_in: []
auth_types:
- token
- http
description: Platform9 Private Cloud Director uses OpenStack Keystone v3 identity. Clients authenticate at POST https://{host}/keystone/v3/auth/tokens to obtain a token, then present it on subsequent requests via the X-Auth-Token header. Machine-to- machine automation uses Application Credentials (id/name/secret) rather than user passwords. Multi-factor (TOTP) and Enterprise SSO (SAML/OIDC via Dex) are supported. Tokens can be scoped to a project, domain, or system.
kind: authentication
layout: security
method: searched
name: Platform9 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Platform9 secures its APIs with token and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Platform9
provider_slug: platform9
scheme_count: 5
schemes:
- description: Keystone-issued auth token presented on every authenticated request.
  in: header
  name: keystoneToken
  parameter: X-Auth-Token
  sources:
  - https://docs.platform9.com/api-docs/identity-service/authentication.md
  type: apiKey
- description: Username/password authentication scoped to a project or domain.
  flow: POST /keystone/v3/auth/tokens (identity method "password")
  name: keystonePassword
  type: password
- description: Non-interactive credential for automation and service-to-service auth; supports restricted flag. Recommended for API/CLI automation.
  fields:
  - id
  - name
  - secret
  flow: POST /keystone/v3/auth/tokens (identity method "application_credential")
  name: applicationCredential
  type: application_credential
- description: Time-based one-time password used as a second factor.
  name: totp
  type: mfa
- description: Corporate single sign-on federated into Keystone.
  name: enterpriseSSO
  protocols:
  - SAML2
  - OIDC
  provider: Dex (github.com/platform9/dex)
  type: federation
slug: platform9-authentication
source_filename: platform9-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.platform9.com/api-docs/identity-service/authentication.md\ndocs: https://docs.platform9.com/api-docs/identity-service/authentication.md\nsummary:\n  types: [token, http]\n  model: openstack-keystone-v3\n  token_header: X-Auth-Token\n  identity_base: https://{host}/keystone/v3\n  auth_methods: [password, token, application_credential, totp]\ndescription: >-\n  Platform9 Private Cloud Director uses OpenStack Keystone v3 identity. Clients\n  authenticate at POST https://{host}/keystone/v3/auth/tokens to obtain a token,\n  then present it on subsequent requests via the X-Auth-Token header. Machine-to-\n  machine automation uses Application Credentials (id/name/secret) rather than\n  user passwords. Multi-factor (TOTP) and Enterprise SSO (SAML/OIDC via Dex) are\n  supported. Tokens can be scoped to a project, domain, or system.\nschemes:\n- name: keystoneToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n\
  \  description: Keystone-issued auth token presented on every authenticated request.\n  sources: [https://docs.platform9.com/api-docs/identity-service/authentication.md]\n- name: keystonePassword\n  type: password\n  flow: POST /keystone/v3/auth/tokens (identity method \"password\")\n  description: Username/password authentication scoped to a project or domain.\n- name: applicationCredential\n  type: application_credential\n  flow: POST /keystone/v3/auth/tokens (identity method \"application_credential\")\n  fields: [id, name, secret]\n  description: >-\n    Non-interactive credential for automation and service-to-service auth;\n    supports restricted flag. Recommended for API/CLI automation.\n- name: totp\n  type: mfa\n  description: Time-based one-time password used as a second factor.\n- name: enterpriseSSO\n  type: federation\n  protocols: [SAML2, OIDC]\n  provider: Dex (github.com/platform9/dex)\n  description: Corporate single sign-on federated into Keystone.\nscoping:\n  - project\
  \ (by id or name, optional domain)\n  - domain (by id or name)\n  - system (all)\nroles: openstack-rbac\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platform9/refs/heads/main/authentication/platform9-authentication.yml
summary_line: token/http · 5 schemes
tags:
- Company
- Infrastructure
- Private Cloud
- OpenStack
- Kubernetes
- Virtualization
- IaaS
- VMware Migration
- Cloud Management
---
