---
api_key_in:
- header
auth_types:
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Interfolio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Interfolio secures its APIs with hmac across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Interfolio
provider_slug: interfolio
scheme_count: 2
schemes:
- algorithm: HMAC-SHA1
  credentials:
  - publicKey
  - privateKey
  - databaseId
  description: Faculty180 Faculty Activity Reporting API request signing. The Authorization header carries the public key and the request signature; a Timestamp header and an INTF-DatabaseID header identify the institution database. Key pairs are issued by Interfolio per institution.
  headers:
    authorization: INTF {publicKey}:{signature}
    database_id: INTF-DatabaseID
    timestamp: Timestamp
  in: header
  name: HMAC (Faculty180)
  sources:
  - https://www.faculty180.com/api_docs
  type: hmac
- credentials:
  - publicKey
  - privateKey
  - tenantId
  description: Interfolio Core, Faculty Search, and Review-Promotion-Tenure REST + GraphQL API request signing. The client is instantiated with restUrl (logic.interfolio.com), graphQlUrl (caasbox.interfolio.com), tenantId, publicKey, and privateKey; each request is HMAC-signed. Intended for backend/middleware integrations, not public front-end use (private key required).
  graphql_url: https://caasbox.interfolio.com
  in: header
  name: HMAC (Core / Search / RPT)
  rest_url: https://logic.interfolio.com
  sources:
  - https://sas-irad.github.io/interfolio-api/
  type: hmac
slug: interfolio-authentication
source_filename: interfolio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.faculty180.com/api_docs\ndocs:\n- https://www.faculty180.com/api_docs\n- https://faculty180.interfolio.com/swagger/ui/\n- https://sas-irad.github.io/interfolio-api/\nsummary:\n  types: [hmac]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Interfolio does not use OAuth2 or API-key bearer tokens. Both the Faculty180\n    (Faculty Activity Reporting) API and the Core/Search/RPT API authenticate each\n    request with an HMAC-SHA signature computed over the request using an\n    Interfolio-issued public/private key pair, scoped to a tenant (numeric tenantId)\n    or a per-institution database ID. Authorization is enforced server-side by the\n    Interfolio permissioning infrastructure for the identified tenant.\nschemes:\n- name: HMAC (Faculty180)\n  type: hmac\n  in: header\n  description: >-\n    Faculty180 Faculty Activity Reporting API request signing. The Authorization\n    header carries the public\
  \ key and the request signature; a Timestamp header and\n    an INTF-DatabaseID header identify the institution database. Key pairs are issued\n    by Interfolio per institution.\n  headers:\n    authorization: 'INTF {publicKey}:{signature}'\n    timestamp: 'Timestamp'\n    database_id: 'INTF-DatabaseID'\n  algorithm: HMAC-SHA1\n  credentials: [publicKey, privateKey, databaseId]\n  sources: [https://www.faculty180.com/api_docs]\n- name: HMAC (Core / Search / RPT)\n  type: hmac\n  in: header\n  description: >-\n    Interfolio Core, Faculty Search, and Review-Promotion-Tenure REST + GraphQL API\n    request signing. The client is instantiated with restUrl (logic.interfolio.com),\n    graphQlUrl (caasbox.interfolio.com), tenantId, publicKey, and privateKey; each\n    request is HMAC-signed. Intended for backend/middleware integrations, not public\n    front-end use (private key required).\n  credentials: [publicKey, privateKey, tenantId]\n  rest_url: https://logic.interfolio.com\n  graphql_url:\
  \ https://caasbox.interfolio.com\n  sources: [https://sas-irad.github.io/interfolio-api/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/authentication/interfolio-authentication.yml
summary_line: hmac · 2 schemes
tags:
- Company
- Education
- Higher Education
- Faculty Information System
- Faculty Activity Reporting
- Review Promotion Tenure
- Academic
- Research
---
