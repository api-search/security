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
- filename: netdata-alerts-api-openapi.yml
  format: yaml
  label: Netdata alerts API
  slug: netdata-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-alerts-api-openapi.yml
- filename: netdata-authentication-api-openapi.yml
  format: yaml
  label: Netdata authentication API
  slug: netdata-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-authentication-api-openapi.yml
- filename: netdata-badges-api-openapi.yml
  format: yaml
  label: Netdata badges API
  slug: netdata-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-badges-api-openapi.yml
- filename: netdata-charts-api-openapi.yml
  format: yaml
  label: Netdata charts API
  slug: netdata-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-charts-api-openapi.yml
- filename: netdata-claiming-api-openapi.yml
  format: yaml
  label: Netdata claiming API
  slug: netdata-claiming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-claiming-api-openapi.yml
- filename: netdata-config-api-openapi.yml
  format: yaml
  label: Netdata config API
  slug: netdata-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-config-api-openapi.yml
- filename: netdata-contexts-api-openapi.yml
  format: yaml
  label: Netdata contexts API
  slug: netdata-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-contexts-api-openapi.yml
- filename: netdata-data-api-openapi.yml
  format: yaml
  label: Netdata data API
  slug: netdata-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-data-api-openapi.yml
- filename: netdata-dyncfg-api-openapi.yml
  format: yaml
  label: Netdata dyncfg API
  slug: netdata-dyncfg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-dyncfg-api-openapi.yml
- filename: netdata-functions-api-openapi.yml
  format: yaml
  label: Netdata functions API
  slug: netdata-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-functions-api-openapi.yml
- filename: netdata-management-api-openapi.yml
  format: yaml
  label: Netdata management API
  slug: netdata-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-management-api-openapi.yml
- filename: netdata-nodes-api-openapi.yml
  format: yaml
  label: Netdata nodes API
  slug: netdata-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-nodes-api-openapi.yml
- filename: netdata-registry-api-openapi.yml
  format: yaml
  label: Netdata registry API
  slug: netdata-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-registry-api-openapi.yml
- filename: netdata-settings-api-openapi.yml
  format: yaml
  label: Netdata settings API
  slug: netdata-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-settings-api-openapi.yml
- filename: netdata-streaming-api-openapi.yml
  format: yaml
  label: Netdata streaming API
  slug: netdata-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-streaming-api-openapi.yml
- filename: netdata-variables-api-openapi.yml
  format: yaml
  label: Netdata variables API
  slug: netdata-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-variables-api-openapi.yml
- filename: netdata-versions-api-openapi.yml
  format: yaml
  label: Netdata versions API
  slug: netdata-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-versions-api-openapi.yml
- filename: netdata-webrtc-api-openapi.yml
  format: yaml
  label: Netdata webrtc API
  slug: netdata-webrtc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-webrtc-api-openapi.yml
- filename: netdata-weights-api-openapi.yml
  format: yaml
  label: Netdata weights API
  slug: netdata-weights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-weights-api-openapi.yml
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
