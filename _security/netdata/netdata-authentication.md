---
api_key_in:
- header
api_specs:
- filename: netdata-swagger.yaml
  format: yaml
  label: Netdata Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/netdata/netdata/master/src/web/api/netdata-swagger.yaml
- filename: netdata-cloud-api-openapi.yml
  format: yaml
  label: Netdata Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-cloud-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Netdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Netdata secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Netdata
provider_slug: netdata
scheme_count: 2
schemes:
- description: 'Bearer token authentication for API access when bearer protection is enabled.


    **How to obtain a token:**

    1. Token must be obtained via `/api/v3/bearer_get_token` endpoint

    2. This endpoint is ACLK-only (requires Netdata Cloud access)

    3. Token includes role-based access control and expiration time


    **How to use:**

    ```

    Authorization: Bearer <token>

    ```


    **When required:**

    - When bearer protection is'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/netdata-agent-api-openapi.yml
  - openapi/netdata-cloud-api-openapi.yml
  type: http
- description: "IP-based Access Control List restrictions (informational only).\n\n**Configuration:**\nAPIs are subject to IP-based ACL restrictions configured in `netdata.conf`:\n\n```conf\n[web]\n    allow dashboard from = *\n    allow badges from = *\n    allow management from = localhost\n```\n\n**ACL Categories:**\n- `allow dashboard from` - Controls access to metrics, alerts, nodes, functions, config APIs\n- `allow badge"
  in: header
  name: ipAcl
  parameter: X-Forwarded-For
  sources:
  - openapi/netdata-agent-api-openapi.yml
  type: apiKey
slug: netdata-authentication
source_filename: netdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/netdata-agent-api-openapi.yml, openapi/netdata-cloud-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token authentication for API access when bearer protection is enabled.\n\n    **How to obtain a token:**\n    1. Token must be obtained via `/api/v3/bearer_get_token` endpoint\n    2. This endpoint is ACLK-only (requires Netdata Cloud access)\n    3. Token includes role-based access control and expiration time\n\n    **How to use:**\n    ```\n    Authorization: Bearer <token>\n    ```\n\n    **When required:**\n    - When bearer protection is\n  sources:\n  - openapi/netdata-agent-api-openapi.yml\n  - openapi/netdata-cloud-api-openapi.yml\n- name: ipAcl\n  type: apiKey\n  in: header\n  parameter: X-Forwarded-For\n  description: |-\n    IP-based Access Control List restrictions (informational\
  \ only).\n\n    **Configuration:**\n    APIs are subject to IP-based ACL restrictions configured in `netdata.conf`:\n\n    ```conf\n    [web]\n        allow dashboard from = *\n        allow badges from = *\n        allow management from = localhost\n    ```\n\n    **ACL Categories:**\n    - `allow dashboard from` - Controls access to metrics, alerts, nodes, functions, config APIs\n    - `allow badge\n  sources:\n  - openapi/netdata-agent-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/authentication/netdata-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Monitoring
- Observability
- Infrastructure
- Metrics
- Alerts
- Real-Time
- APM
- DevOps
---
