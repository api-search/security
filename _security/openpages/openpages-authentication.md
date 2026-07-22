---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Openpages Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenPages secures its APIs with oauth2 and http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenPages
provider_slug: openpages
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'IBM Cloud IAM access token presented as Authorization: Bearer <token>. Tokens are obtained by exchanging an IBM Cloud IAM API key at the IAM token service.'
  name: iam-bearer
  scheme: bearer
  sources:
  - https://cloud.ibm.com/docs/openpages?topic=openpages-iam-openpages
  token_endpoint: https://iam.cloud.ibm.com/identity/token
  type: http
slug: openpages-authentication
source_filename: openpages-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://cloud.ibm.com/docs/openpages?topic=openpages-iam-openpages\ndocs: https://cloud.ibm.com/docs/openpages?topic=openpages-iam-openpages\nsummary:\n  types: [oauth2, http]\n  model: IBM Cloud Identity and Access Management (IAM)\n  token_type: IAM bearer access token\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Access to OpenPages service instances is controlled by IBM Cloud Identity and\n  Access Management (IAM); further, finer-grained access is managed within the\n  OpenPages application itself. Calls to the OpenPages REST API require the\n  caller to hold the OpenPages \"User\" service access role (crn service role\n  GRCUser) and to present an IAM bearer access token. IAM API keys are exchanged\n  for bearer tokens at the IBM Cloud IAM token endpoint. Users and groups are\n  synchronized from IBM Cloud IAM into OpenPages; identities can be federated.\nschemes:\n- name: iam-bearer\n  type: http\n  scheme: bearer\n\
  \  bearerFormat: JWT\n  description: >-\n    IBM Cloud IAM access token presented as Authorization: Bearer <token>.\n    Tokens are obtained by exchanging an IBM Cloud IAM API key at the IAM token\n    service.\n  token_endpoint: https://iam.cloud.ibm.com/identity/token\n  sources: ['https://cloud.ibm.com/docs/openpages?topic=openpages-iam-openpages']\nroles:\n- name: OpenPages User\n  crn: crn:v1:bluemix:public:openpages::::serviceRole:GRCUser\n  grants: Log in to OpenPages and make calls to the OpenPages REST API.\n- name: Viewer\n  crn: crn:v1:bluemix:public:openpages::::serviceRole:Viewer\n- name: Operator\n  crn: crn:v1:bluemix:public:openpages::::serviceRole:Operator\n- name: Editor\n  crn: crn:v1:bluemix:public:openpages::::serviceRole:Editor\n- name: Administrator\n  crn: crn:v1:bluemix:public:openpages::::serviceRole:Administrator\nnetwork_controls:\n  ip_allowlisting: >-\n    Optional per-instance IP allowlisting (IPv4/IPv6 addresses or CIDR ranges)\n    restricts which clients\
  \ can log in and access the API. By default all IP\n    addresses are allowed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpages/refs/heads/main/authentication/openpages-authentication.yml
summary_line: oauth2/http · 1 scheme
tags:
- Company
- B2B
- Governance
- Risk
- Compliance
- GRC
- Regulatory Compliance
- Risk Management
- Enterprise Software
- watsonx
- Audit
---
