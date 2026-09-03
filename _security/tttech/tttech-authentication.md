---
api_key_in:
- header
api_specs:
- filename: tttech-nerve-management-system-openapi.yml
  format: yaml
  label: Nerve Management System API
  slug: nerve-management-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tttech/refs/heads/main/openapi/tttech-nerve-management-system-openapi.yml
- filename: tttech-nerve-node-openapi.yml
  format: yaml
  label: Nerve Node API
  slug: nerve-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tttech/refs/heads/main/openapi/tttech-nerve-node-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tttech Authentication
name_suffix: Authentication
oauth_flows: []
overview: TTTech secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TTTech
provider_slug: tttech
scheme_count: 4
schemes:
- in: header
  name: sessionId
  parameter: sessionId
  sources:
  - openapi/tttech-nerve-management-system-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/tttech-nerve-management-system-openapi.yml
  - openapi/tttech-nerve-node-openapi.yml
  type: http
- in: header
  name: cookieAuth
  parameter: cookie
  sources:
  - openapi/tttech-nerve-management-system-openapi.yml
  - openapi/tttech-nerve-node-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tttech-nerve-management-system-openapi.yml
  type: http
slug: tttech-authentication
source_filename: tttech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: openapi/tttech-nerve-management-system-openapi.yml, openapi/tttech-nerve-node-openapi.yml, https://docs.nerve.cloud/user_guide/management_system/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: 0\nschemes:\n- name: sessionId\n  type: apiKey\n  in: header\n  parameter: sessionId\n  sources:\n  - openapi/tttech-nerve-management-system-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/tttech-nerve-management-system-openapi.yml\n  - openapi/tttech-nerve-node-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: header\n  parameter: cookie\n  sources:\n  - openapi/tttech-nerve-management-system-openapi.yml\n  - openapi/tttech-nerve-node-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tttech-nerve-management-system-openapi.yml\ndocs:\n- https://docs.nerve.cloud/user_guide/management_system/users/\n- https://docs.nerve.cloud/user_guide/management_system/mfa/\n\
  - https://docs.nerve.cloud/user_guide/management_system/ldap/\n- https://docs.nerve.cloud/user_guide/management_system/roles/\n- https://docs.nerve.cloud/user_guide/local_ui/permissions_and_users/\nmodel:\n  primary: session\n  detail: POST /auth/login exchanges username and password for a session. The Management System's global security requirement\n    is the sessionId apiKey header; a cookie header is accepted as an alternative and the Node API uses the cookie header\n    as its global requirement. HTTP basic and HTTP bearer schemes are declared and used by a subset of operations. There is\n    no OAuth 2.0 authorization server, no OpenID Connect discovery document and therefore no scope surface — scopes/ is deliberately\n    absent from this repository.\n  multi_factor:\n    supported: true\n    since: Nerve 2.9.0\n    operations:\n    - mfa_is_enabled\n    - mfa_generate\n    - mfa_activate\n    - mfa_validate\n    - mfa_reset\n    detail: 'TOTP-style: mfa_generate returns the user''s\
  \ secret and a QR code URL, mfa_activate enables it with an activation\n      token, mfa_validate completes login with the code, mfa_reset clears it with a reset token. mfa_is_enabled is unauthenticated\n      and tells a client whether the Management System requires a second factor.'\n    docs: https://docs.nerve.cloud/user_guide/management_system/mfa/\n  directory_federation:\n    supported: true\n    protocol: LDAP\n    operations:\n    - create_ldap_connections\n    - get_ldap_config_details\n    - get_ldap_status\n    - get_default_ldap\n    - activate_deactivate_ldap\n    - test_ldap_connection\n    - ldap_users\n    - ldap_groups\n    detail: TTTech's own IEC 62443-4-2 mapping cites LDAP as the control satisfying CR1.4 identifier management and CR1.5\n      authenticator management, and its security checklist recommends organization-wide credential management through LDAP,\n      with MFA as the fallback when LDAP is not used.\n    docs: https://docs.nerve.cloud/user_guide/management_system/ldap/\n\
  \  authorization:\n    model: roles and permissions\n    detail: Users are assigned roles; roles carry permissions. TTTech maps this to CR2.1 authorization enforcement and CR2.1\n      RE(2) permission mapping to roles. Node accounts can be synchronised from the Management System (Nerve 2.9.0).\n    docs: https://docs.nerve.cloud/user_guide/management_system/roles/\n  session_controls:\n    configurable_since: Nerve 3.1.0\n    mechanism: Node DNA\n    fields:\n    - sessionTimeout\n    - maxSessionsPerUser\n    - maxSSHConnections\n    password_policy:\n    - complexity\n    - lifetime and expiration\n    - expiration warnings\n    docs: https://docs.nerve.cloud/developer_guide/dna/\n  brute_force_protection:\n    supported: true\n    since: Nerve 2.5.0\n    see: rate-limits/tttech-rate-limits.yml\n  credential_handling_warning: The first-party CLI can persist Management System credentials to a plain-text credentials.ini;\n    TTTech flags this in the CLI's own --store-credentials help\
  \ text. TTTech's security checklist also requires that Nerve\n    DNA files contain no credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tttech/refs/heads/main/authentication/tttech-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Industrial IoT
- Edge Computing
- Device Management
- Deterministic Networking
- Time-Sensitive Networking
- Industrial Automation
- Workload Orchestration
- Embedded Systems
- Safety Critical
- OPC UA
- MQTT
- CODESYS
- IEC 62443
---
