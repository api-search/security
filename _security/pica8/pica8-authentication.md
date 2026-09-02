---
api_key_in: []
api_specs:
- filename: pica8-backup-api-openapi.yml
  format: yaml
  label: Pica8 Backup API
  slug: pica8-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-backup-api-openapi.yml
- filename: pica8-configuration-api-openapi.yml
  format: yaml
  label: Pica8 Configuration API
  slug: pica8-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-configuration-api-openapi.yml
- filename: pica8-configurationfile-api-openapi.yml
  format: yaml
  label: Pica8 Configuration File API
  slug: pica8-configurationfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-configurationfile-api-openapi.yml
- filename: pica8-group-api-openapi.yml
  format: yaml
  label: Pica8 Group API
  slug: pica8-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-group-api-openapi.yml
- filename: pica8-job-api-openapi.yml
  format: yaml
  label: Pica8 Job API
  slug: pica8-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-job-api-openapi.yml
- filename: pica8-license-api-openapi.yml
  format: yaml
  label: Pica8 License API
  slug: pica8-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-license-api-openapi.yml
- filename: pica8-playbook-api-openapi.yml
  format: yaml
  label: Pica8 Playbook API
  slug: pica8-playbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-playbook-api-openapi.yml
- filename: pica8-settings-api-openapi.yml
  format: yaml
  label: Pica8 Settings API
  slug: pica8-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-settings-api-openapi.yml
- filename: pica8-switch-api-openapi.yml
  format: yaml
  label: Pica8 Switch API
  slug: pica8-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-switch-api-openapi.yml
- filename: pica8-template-api-openapi.yml
  format: yaml
  label: Pica8 Template API
  slug: pica8-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-template-api-openapi.yml
- filename: pica8-token-api-openapi.yml
  format: yaml
  label: Pica8 Token API
  slug: pica8-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-token-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Pica8 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pica8 secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pica8
provider_slug: pica8
scheme_count: 3
schemes:
- api: Pica8 AmpCon Network Controller API
  bearerFormat: JWT
  format: 'Authorization: Bearer <generated-token>'
  header: Authorization
  in: header
  invalid_token_behaviour: Expired or invalid tokens are rejected with the message "Invalid Token".
  known_issues:
  - 'AmpCon 1.12.1 release notes, ticket 857: "AmpCon API JWT token shows invalid since requests will be routed to different backend instances." Fixed in 1.12.1; operators on earlier multi-instance deployments saw spurious invalid-token errors.'
  name: bearerAuth
  privilege_requirement: 'Only "superadmin" level AmpCon users may mint a token or call the API. A lower-privileged user receives {"msg": "Permission denied, you should use \"superadmin\" user"}. This is the whole authorization model - the API has no scopes and no per-operation permissions.'
  scheme: bearer
  sources:
  - openapi/pica8-ampcon-openapi.yml
  - https://pica8-fs.atlassian.net/wiki/spaces/ampcon/pages/753668/AmpCon+API+document
  token_credential: AmpCon web login username + password, posted as JSON
  token_endpoint: POST https://{ampcon-server-ip}/token
  type: http
- api: PICOS RESTCONF / NETCONF / gNMI Device API
  description: PICOS RESTCONF supports HTTP Basic authentication only. The username and password are the accounts configured for authentication on the RESTCONF server (the switch itself). Credentials are carried in the HTTPS request from the RESTCONF client.
  header: Authorization
  in: header
  name: restconfBasic
  scheme: basic
  sources:
  - https://pica8-fs.atlassian.net/wiki/spaces/Picos48white/pages/1157576061/Introduction+of+RESTCONF
  transport_note: RESTCONF defaults to ports 80/443, which collide with the picos-web service. When picos-web is enabled a custom RESTCONF port must be configured (`set protocols restconf port`) or RESTCONF returns authentication errors.
  type: http
- api: PICOS RESTCONF / NETCONF / gNMI Device API
  description: NETCONF sessions on a PICOS switch are opened over SSH and authorized through the switch's AAA configuration. Pica8 documents that authenticated RADIUS and TACACS+ users can reach the switch over NETCONF.
  name: netconfSsh
  scheme: ssh-with-aaa
  sources:
  - https://pica8-fs.atlassian.net/wiki/spaces/Picos48white/pages/1157576481/Configuring+NETCONF
  type: other
slug: pica8-authentication
source_filename: pica8-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  Pica8 AmpCon API document (https://pica8-fs.atlassian.net/wiki/spaces/ampcon/pages/753668/AmpCon+API+document,\n  attachment \"AmpCon 1.12.0 API document 20230625.docx\"), PICOS 4.8 \"Introduction of RESTCONF\"\n  (https://pica8-fs.atlassian.net/wiki/spaces/Picos48white/pages/1157576061/Introduction+of+RESTCONF) and\n  \"Configuring NETCONF\" (https://pica8-fs.atlassian.net/wiki/spaces/Picos48white/pages/1157576481/Configuring+NETCONF),\n  cross-checked against openapi/pica8-ampcon-openapi.yml\nsummary:\n  types:\n  - http\n  hosted_identity_provider: false\n  note: >-\n    Every Pica8 programmatic surface authenticates against the customer's own deployment. There is no Pica8-operated\n    identity provider, no OAuth 2.0 authorization server, no API key issuance portal and no /.well-known/\n    OpenID or OAuth metadata anywhere on pica8.com - all five paths were probed on 2026-08-26 and returned 404.\nschemes:\n- name:\
  \ bearerAuth\n  api: Pica8 AmpCon Network Controller API\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <generated-token>'\n  token_endpoint: POST https://{ampcon-server-ip}/token\n  token_credential: AmpCon web login username + password, posted as JSON\n  privilege_requirement: >-\n    Only \"superadmin\" level AmpCon users may mint a token or call the API. A lower-privileged user receives\n    {\"msg\": \"Permission denied, you should use \\\"superadmin\\\" user\"}. This is the whole authorization model -\n    the API has no scopes and no per-operation permissions.\n  invalid_token_behaviour: 'Expired or invalid tokens are rejected with the message \"Invalid Token\".'\n  known_issues:\n  - >-\n    AmpCon 1.12.1 release notes, ticket 857: \"AmpCon API JWT token shows invalid since requests will be routed\n    to different backend instances.\" Fixed in 1.12.1; operators on earlier multi-instance deployments\
  \ saw\n    spurious invalid-token errors.\n  sources:\n  - openapi/pica8-ampcon-openapi.yml\n  - https://pica8-fs.atlassian.net/wiki/spaces/ampcon/pages/753668/AmpCon+API+document\n- name: restconfBasic\n  api: PICOS RESTCONF / NETCONF / gNMI Device API\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  description: >-\n    PICOS RESTCONF supports HTTP Basic authentication only. The username and password are the accounts configured\n    for authentication on the RESTCONF server (the switch itself). Credentials are carried in the HTTPS request\n    from the RESTCONF client.\n  transport_note: >-\n    RESTCONF defaults to ports 80/443, which collide with the picos-web service. When picos-web is enabled a custom\n    RESTCONF port must be configured (`set protocols restconf port`) or RESTCONF returns authentication errors.\n  sources:\n  - https://pica8-fs.atlassian.net/wiki/spaces/Picos48white/pages/1157576061/Introduction+of+RESTCONF\n- name: netconfSsh\n  api: PICOS\
  \ RESTCONF / NETCONF / gNMI Device API\n  type: other\n  scheme: ssh-with-aaa\n  description: >-\n    NETCONF sessions on a PICOS switch are opened over SSH and authorized through the switch's AAA configuration.\n    Pica8 documents that authenticated RADIUS and TACACS+ users can reach the switch over NETCONF.\n  sources:\n  - https://pica8-fs.atlassian.net/wiki/spaces/Picos48white/pages/1157576481/Configuring+NETCONF\noauth:\n  present: false\n  reason: >-\n    No OAuth 2.0 or OpenID Connect surface is documented or served. /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server both returned 404 on www.pica8.com on 2026-08-26. scopes/ is\n    therefore intentionally absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/authentication/pica8-authentication.yml
summary_line: http · 3 schemes
tags:
- Networking
- Open Networking
- Software Defined Networking
- Network Automation
- Network Operating System
- white-box-switching
- Network Management
- Campus Networking
- Data Center Networking
- RESTCONF
- NETCONF
- Telemetry
---
