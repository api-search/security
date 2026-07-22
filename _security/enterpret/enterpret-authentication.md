---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Enterpret Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enterpret secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Enterpret
provider_slug: enterpret
scheme_count: 2
schemes:
- description: Recommended authentication, managed through each MCP host's authorization flow.
  name: oauth
  sources:
  - https://helpcenter.enterpret.com/en/articles/12665166-enterpret-mcp-server
  type: oauth2
- description: 'Long-lived bearer auth token generated in the Enterpret dashboard (Settings > Enterpret MCP > Generate under Auth Token). Sent as ''Authorization: Bearer <token>''. Tokens expire after 6 months.'
  name: bearerToken
  scheme: bearer
  sources:
  - https://helpcenter.enterpret.com/en/articles/12665166-enterpret-mcp-server
  type: http
slug: enterpret-authentication
source_filename: enterpret-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://helpcenter.enterpret.com/en/articles/12665166-enterpret-mcp-server\ndocs: https://helpcenter.enterpret.com/en/collections/9060203-enterpret-mcp\nnote: >-\n  Enterpret does not publish a public OpenAPI. Auth model is documented for the\n  Enterpret MCP server (wisdom-api.enterpret.com), which fronts the customer\n  intelligence / Wisdom graph. OAuth is the recommended flow; a long-lived\n  bearer auth token is the alternative.\nsummary:\n  types:\n  - oauth2\n  - http\n  http_schemes:\n  - bearer\n  recommended: oauth2\nschemes:\n- name: oauth\n  type: oauth2\n  description: Recommended authentication, managed through each MCP host's authorization flow.\n  sources:\n  - https://helpcenter.enterpret.com/en/articles/12665166-enterpret-mcp-server\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Long-lived bearer auth token generated in the Enterpret dashboard\n    (Settings > Enterpret MCP >\
  \ Generate under Auth Token). Sent as\n    'Authorization: Bearer <token>'. Tokens expire after 6 months.\n  sources:\n  - https://helpcenter.enterpret.com/en/articles/12665166-enterpret-mcp-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enterpret/refs/heads/main/authentication/enterpret-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Customer Intelligence
- Customer Feedback
- Voice of Customer
- Customer Experience
- Analytics
- Artificial Intelligence
- MCP
- SaaS
---
