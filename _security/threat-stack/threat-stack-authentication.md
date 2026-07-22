---
api_key_in:
- header
auth_types:
- hawk
description: ''
kind: authentication
layout: security
method: searched
name: Threat Stack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Threat Stack secures its APIs with hawk across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Threat Stack
provider_slug: threat-stack
scheme_count: 1
schemes:
- credentials:
  - description: User ID of the API key holder.
    id: TS_USER_ID
    maps_to: HAWK Auth ID
  - description: API key for the user specified by TS_USER_ID.
    id: TS_API_KEY
    maps_to: HAWK Auth Key
  - description: Organization ID of the organization to access.
    id: TS_ORGANIZATION_ID
    maps_to: HAWK Ext
  description: The Threat Stack V2 REST API authenticates every request with HAWK, an HMAC-based HTTP authentication scheme. The signature is computed from the caller's API key, and the request carries a signed Authorization header so the platform can verify the sender.
  name: hawk
  scheme: hawk
  sources:
  - docs
  type: http
slug: threat-stack-authentication
source_filename: threat-stack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://clouddocs.f5.com/training/community/threat-stack/html/class2/Threat_Stack_API.html\ndocs: https://clouddocs.f5.com/training/community/threat-stack/html/class2/Threat_Stack_API.html\nsummary:\n  types: [hawk]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: hawk\n    type: http\n    scheme: hawk\n    description: >-\n      The Threat Stack V2 REST API authenticates every request with HAWK, an\n      HMAC-based HTTP authentication scheme. The signature is computed from the\n      caller's API key, and the request carries a signed Authorization header so\n      the platform can verify the sender.\n    credentials:\n      - id: TS_USER_ID\n        maps_to: HAWK Auth ID\n        description: User ID of the API key holder.\n      - id: TS_API_KEY\n        maps_to: HAWK Auth Key\n        description: API key for the user specified by TS_USER_ID.\n      - id: TS_ORGANIZATION_ID\n        maps_to: HAWK Ext\n \
  \       description: Organization ID of the organization to access.\n    sources: [docs]\nnotes: >-\n  Derived from published F5/Threat Stack documentation rather than an OpenAPI\n  spec (no machine-readable spec is published). Threat Stack is now F5\n  Distributed Cloud App Infrastructure Protection (AIP); the api.threatstack.com\n  host is decommissioned.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threat-stack/refs/heads/main/authentication/threat-stack-authentication.yml
summary_line: hawk · 1 scheme
tags:
- Company
- Security
- Cloud Security
- Cloud Monitoring
- Intrusion Detection
- Compliance
- Observability
- DevSecOps
- Containers
- Kubernetes
---
