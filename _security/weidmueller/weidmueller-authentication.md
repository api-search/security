---
anonymous_access: false
api_key_in: []
api_specs:
- filename: weidmueller-variable-nats-asyncapi.yml
  format: yaml
  label: Weidmüller u-OS Data Hub Variable-NATS API
  slug: u-os-data-hub-variable-nats-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/asyncapi/weidmueller-variable-nats-asyncapi.yml
- filename: weidmueller-consumer-api-openapi.yml
  format: yaml
  label: Weidmüller Consumer API
  slug: weidmueller-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-consumer-api-openapi.yml
- filename: weidmueller-firewall-api-openapi.yml
  format: yaml
  label: Weidmüller Firewall API
  slug: weidmueller-firewall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-firewall-api-openapi.yml
- filename: weidmueller-logging-api-openapi.yml
  format: yaml
  label: Weidmüller Logging API
  slug: weidmueller-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-logging-api-openapi.yml
- filename: weidmueller-network-api-openapi.yml
  format: yaml
  label: Weidmüller Network API
  slug: weidmueller-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-network-api-openapi.yml
- filename: weidmueller-operations-api-openapi.yml
  format: yaml
  label: Weidmüller Operations API
  slug: weidmueller-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-operations-api-openapi.yml
- filename: weidmueller-ping-api-openapi.yml
  format: yaml
  label: Weidmüller Ping API
  slug: weidmueller-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-ping-api-openapi.yml
- filename: weidmueller-realtime-api-openapi.yml
  format: yaml
  label: Weidmüller Realtime API
  slug: weidmueller-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-realtime-api-openapi.yml
- filename: weidmueller-recovery-api-openapi.yml
  format: yaml
  label: Weidmüller Recovery API
  slug: weidmueller-recovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-recovery-api-openapi.yml
- filename: weidmueller-security-api-openapi.yml
  format: yaml
  label: Weidmüller Security API
  slug: weidmueller-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-security-api-openapi.yml
- filename: weidmueller-serial-interfaces-api-openapi.yml
  format: yaml
  label: Weidmüller Serial Interfaces API
  slug: weidmueller-serial-interfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-serial-interfaces-api-openapi.yml
- filename: weidmueller-syslog-api-openapi.yml
  format: yaml
  label: Weidmüller Syslog API
  slug: weidmueller-syslog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-syslog-api-openapi.yml
- filename: weidmueller-system-api-openapi.yml
  format: yaml
  label: Weidmüller System API
  slug: weidmueller-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-system-api-openapi.yml
- filename: weidmueller-time-api-openapi.yml
  format: yaml
  label: Weidmüller Time API
  slug: weidmueller-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-time-api-openapi.yml
- filename: weidmueller-update-api-openapi.yml
  format: yaml
  label: Weidmüller Update API
  slug: weidmueller-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-update-api-openapi.yml
- filename: weidmueller-open-api-api-openapi.yml
  format: yaml
  label: Weidmüller Open API
  slug: weidmueller-open-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-open-api-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Weidmueller Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Weidmüller secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Weidmüller
provider_slug: weidmueller
scheme_count: 1
schemes:
- description: The HTTP API uses the OAuth2 client credentials flow.
  flows:
  - flow: clientCredentials
    scopes: 20
    tokenUrl: /oauth2/token
  name: OAuth2
  sources:
  - openapi/weidmueller-administration-openapi.yml
  - openapi/weidmueller-variable-http-openapi.yml
  type: oauth2
slug: weidmueller-authentication
source_filename: weidmueller-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/weidmueller-administration-openapi.yml, openapi/weidmueller-variable-http-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n    scopes: 20\n  description: The HTTP API uses the OAuth2 client credentials flow.\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n  - openapi/weidmueller-variable-http-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/authentication/weidmueller-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Industrial Automation
- Industrial Connectivity
- Edge Computing
- IIoT
- u-OS
- Manufacturing
---
