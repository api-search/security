---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: interfolio-activities-api-openapi.yml
  format: yaml
  label: Interfolio Activities API
  slug: interfolio-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activities-api-openapi.yml
- filename: interfolio-activity-classifications-api-openapi.yml
  format: yaml
  label: Interfolio Activity Classifications API
  slug: interfolio-activity-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activity-classifications-api-openapi.yml
- filename: interfolio-activity-input-api-openapi.yml
  format: yaml
  label: Interfolio Activity Input API
  slug: interfolio-activity-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activity-input-api-openapi.yml
- filename: interfolio-courses-api-openapi.yml
  format: yaml
  label: Interfolio Courses API
  slug: interfolio-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-courses-api-openapi.yml
- filename: interfolio-download-attachments-api-openapi.yml
  format: yaml
  label: Interfolio Download Attachments API
  slug: interfolio-download-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-download-attachments-api-openapi.yml
- filename: interfolio-emails-api-openapi.yml
  format: yaml
  label: Interfolio Emails API
  slug: interfolio-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-emails-api-openapi.yml
- filename: interfolio-evaluations-api-openapi.yml
  format: yaml
  label: Interfolio Evaluations API
  slug: interfolio-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-evaluations-api-openapi.yml
- filename: interfolio-faculty-classifications-api-openapi.yml
  format: yaml
  label: Interfolio Faculty Classifications API
  slug: interfolio-faculty-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-faculty-classifications-api-openapi.yml
- filename: interfolio-faq-api-openapi.yml
  format: yaml
  label: Interfolio FAQ API
  slug: interfolio-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-faq-api-openapi.yml
- filename: interfolio-permissions-api-openapi.yml
  format: yaml
  label: Interfolio Permissions API
  slug: interfolio-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-permissions-api-openapi.yml
- filename: interfolio-sections-api-openapi.yml
  format: yaml
  label: Interfolio Sections API
  slug: interfolio-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-sections-api-openapi.yml
- filename: interfolio-sso-api-openapi.yml
  format: yaml
  label: Interfolio SSO API
  slug: interfolio-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-sso-api-openapi.yml
- filename: interfolio-terms-api-openapi.yml
  format: yaml
  label: Interfolio Terms API
  slug: interfolio-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-terms-api-openapi.yml
- filename: interfolio-units-api-openapi.yml
  format: yaml
  label: Interfolio Units API
  slug: interfolio-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-units-api-openapi.yml
- filename: interfolio-user-data-api-openapi.yml
  format: yaml
  label: Interfolio User Data API
  slug: interfolio-user-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-user-data-api-openapi.yml
- filename: interfolio-users-api-openapi.yml
  format: yaml
  label: Interfolio Users API
  slug: interfolio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-users-api-openapi.yml
- filename: interfolio-vitas-api-openapi.yml
  format: yaml
  label: Interfolio Vitas API
  slug: interfolio-vitas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-vitas-api-openapi.yml
auth_types:
- hmac
description: ''
kind: authentication
layout: security
mechanism_count: 2
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
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.faculty180.com/api_docs\ndocs: https://www.faculty180.com/api_docs\nsummary:\n  types:\n  - hmac\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: Interfolio does not use OAuth2 or API-key bearer tokens. Both the Faculty180\n    (Faculty Activity Reporting) API and the Core/Search/RPT API authenticate each\n    request with an HMAC-SHA signature computed over the request using an Interfolio-issued\n    public/private key pair, scoped to a tenant (numeric tenantId) or a per-institution\n    database ID. Authorization is enforced server-side by the Interfolio permissioning\n    infrastructure for the identified tenant.\nschemes:\n- name: HMAC (Faculty180)\n  type: hmac\n  in: header\n  description: Faculty180 Faculty Activity Reporting API request signing. The Authorization\n    header carries the public key and the request signature; a Timestamp header and\n    an INTF-DatabaseID header identify the institution\
  \ database. Key pairs are issued\n    by Interfolio per institution.\n  headers:\n    authorization: INTF {publicKey}:{signature}\n    timestamp: Timestamp\n    database_id: INTF-DatabaseID\n  algorithm: HMAC-SHA1\n  credentials:\n  - publicKey\n  - privateKey\n  - databaseId\n  sources:\n  - https://www.faculty180.com/api_docs\n- name: HMAC (Core / Search / RPT)\n  type: hmac\n  in: header\n  description: Interfolio Core, Faculty Search, and Review-Promotion-Tenure REST +\n    GraphQL API request signing. The client is instantiated with restUrl (logic.interfolio.com),\n    graphQlUrl (caasbox.interfolio.com), tenantId, publicKey, and privateKey; each\n    request is HMAC-signed. Intended for backend/middleware integrations, not public\n    front-end use (private key required).\n  credentials:\n  - publicKey\n  - privateKey\n  - tenantId\n  rest_url: https://logic.interfolio.com\n  graphql_url: https://caasbox.interfolio.com\n  sources:\n  - https://sas-irad.github.io/interfolio-api/\n\
  docs_additional:\n- https://faculty180.interfolio.com/swagger/ui/\n- https://sas-irad.github.io/interfolio-api/\n"
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
