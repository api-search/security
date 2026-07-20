---
api_key_in:
- header
- query
auth_types:
- apiKey
- http
description: The CloudHealth Platform REST API authenticates every request with a per-user API Key — a globally unique identifier (GUID) that CloudHealth generates for each user from their profile settings in the platform. There is no OAuth flow; the same key is presented on every call and the API enforces the same authentication and role/authorization checks as the CloudHealth Platform UI, so a key only sees data scoped to that user's organization and role. The key may be supplied either as an HTTP bearer token or as an api_key query parameter.
kind: authentication
layout: security
method: searched
name: Cloudhealth Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudHealth Technologies secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CloudHealth Technologies
provider_slug: cloudhealth-technologies
scheme_count: 2
schemes:
- description: 'Preferred method. Send the API Key as a bearer token in the Authorization header: `Authorization: Bearer <API_KEY>`.'
  name: BearerApiKey
  scheme: bearer
  sources:
  - https://apidocs.cloudhealthtech.com/
  type: http
- description: 'Alternative method. Append the API Key as a query parameter: `?api_key=<API_KEY>`.'
  in: query
  name: ApiKeyQuery
  parameter_name: api_key
  sources:
  - https://apidocs.cloudhealthtech.com/
  type: apiKey
slug: cloudhealth-technologies-authentication
source_filename: cloudhealth-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://apidocs.cloudhealthtech.com/\ndocs: https://apidocs.cloudhealthtech.com/\ndescription: >-\n  The CloudHealth Platform REST API authenticates every request with a per-user\n  API Key — a globally unique identifier (GUID) that CloudHealth generates for\n  each user from their profile settings in the platform. There is no OAuth flow;\n  the same key is presented on every call and the API enforces the same\n  authentication and role/authorization checks as the CloudHealth Platform UI, so\n  a key only sees data scoped to that user's organization and role. The key may be\n  supplied either as an HTTP bearer token or as an api_key query parameter.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n  - name: BearerApiKey\n    type: http\n    scheme: bearer\n    description: >-\n      Preferred method. Send the API Key as a bearer token in the Authorization\n      header: `Authorization:\
  \ Bearer <API_KEY>`.\n    sources: [https://apidocs.cloudhealthtech.com/]\n  - name: ApiKeyQuery\n    type: apiKey\n    in: query\n    parameter_name: api_key\n    description: >-\n      Alternative method. Append the API Key as a query parameter:\n      `?api_key=<API_KEY>`.\n    sources: [https://apidocs.cloudhealthtech.com/]\nnotes: >-\n  For POST/PUT requests a `Content-Type: application/json` header is required or\n  the API returns HTTP 422 Unprocessable Entity. Responses are JSON; send\n  `Accept: application/json`.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudhealth-technologies/refs/heads/main/authentication/cloudhealth-technologies-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Enterprise
- Cloud Cost Management
- FinOps
- Cloud Governance
- Multi-Cloud
- Cloud Management Platform
---
