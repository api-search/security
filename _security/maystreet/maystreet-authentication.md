---
api_key_in: []
auth_types:
- http-bearer
- custom-header
description: ''
kind: authentication
layout: security
method: searched
name: Maystreet Authentication
name_suffix: Authentication
oauth_flows: []
overview: MayStreet secures its APIs with http-bearer and custom-header across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MayStreet
provider_slug: maystreet
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'hpq.py builds "Authorization: Bearer <jwt>" by reading a JWT from the file named in the JWT_FILE environment variable, which is provisioned inside the entitled Analytics Workbench environment. Used against the staging endpoint (wss://mdx.stg.maystreet.com) per create_web_socket_client().'
  name: JWT bearer (Workbench-issued)
  scheme: bearer
  sources:
  - https://github.com/maystreet/workbench-hpq-springboard/blob/master/hpq.py
  type: http
- description: 'A proprietary "Authorization: MayStreet-Data-Lake-Secret <hex-secret>" header scheme used against the production HPQ environment (wss://mdx.uat.maystreet.com per hpq.py url()). The springboard embeds a demo secret value verbatim (not reproduced here); real secrets are entitlement-provisioned per customer.'
  in: header
  name: MayStreet-Data-Lake-Secret header
  parameter: Authorization
  sources:
  - https://github.com/maystreet/workbench-hpq-springboard/blob/master/hpq.py
  type: apiKey
slug: maystreet-authentication
source_filename: maystreet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://github.com/maystreet/workbench-hpq-springboard/blob/master/hpq.py\ndocs: https://github.com/maystreet/workbench-hpq-springboard\nsummary:\n  types: [http-bearer, custom-header]\n  self_serve: false\n  public_signup: false\n  note: >-\n    All access is entitlement-managed inside the MayStreet/LSEG Analytics\n    Workbench environment; there is no public developer portal, API key\n    signup, or OAuth documentation. The authentication mechanics below are\n    documented only in the public hpq.py client of the\n    workbench-hpq-springboard repository.\nschemes:\n  - name: JWT bearer (Workbench-issued)\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      hpq.py builds \"Authorization: Bearer <jwt>\" by reading a JWT from the\n      file named in the JWT_FILE environment variable, which is provisioned\n      inside the entitled Analytics Workbench environment. Used against the\n      staging\
  \ endpoint (wss://mdx.stg.maystreet.com) per\n      create_web_socket_client().\n    sources: [https://github.com/maystreet/workbench-hpq-springboard/blob/master/hpq.py]\n  - name: MayStreet-Data-Lake-Secret header\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      A proprietary \"Authorization: MayStreet-Data-Lake-Secret <hex-secret>\"\n      header scheme used against the production HPQ environment\n      (wss://mdx.uat.maystreet.com per hpq.py url()). The springboard embeds\n      a demo secret value verbatim (not reproduced here); real secrets are\n      entitlement-provisioned per customer.\n    sources: [https://github.com/maystreet/workbench-hpq-springboard/blob/master/hpq.py]\nenvironment:\n  - variable: API_SERVER_BASE_URL\n    purpose: Selects production vs staging environment inside Workbench (is_production()).\n  - variable: JWT_FILE\n    purpose: Path to the Workbench-provisioned JWT used for bearer authentication.\ndata_lake:\n  note:\
  \ >-\n    The Market Data Lake is queried through AWS Athena SQL and the Medusa2\n    Python client inside Analytics Workbench; access rides on the Workbench\n    entitlement/session, with no separately documented public credential\n    scheme.\n  sources: [https://github.com/maystreet/workbench-data-lake-springboard]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maystreet/refs/heads/main/authentication/maystreet-authentication.yml
summary_line: http-bearer/custom-header · 2 schemes
tags:
- Financial
- Market Data
- Real-Time
- Trading
- Low Latency
- Tick Data
- Order Book
- Equities
- Options
- Feed Handlers
- PCAP
---
