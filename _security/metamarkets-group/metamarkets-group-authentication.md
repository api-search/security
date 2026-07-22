---
api_key_in: []
auth_types: []
description: Authentication profile for the Metamarkets Real-time Data Ingestion (RDI) API.
kind: authentication
layout: security
method: searched
name: Metamarkets Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metamarkets Group declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Metamarkets Group
provider_slug: metamarkets-group
scheme_count: 1
schemes:
- credentialsProvisioning: manual
  description: RDI endpoints are protected by HTTP Basic authentication. A per-customer username and password are supplied by the Metamarkets data engineer / account representative and passed on every POST (e.g. curl --user <username>:<password>). HTTPS is required so credentials and data are always encrypted in transit.
  header: Authorization
  in: header
  scheme: basic
  transport: https-required
  type: http
slug: metamarkets-group-authentication
source_filename: metamarkets-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "aid: metamarkets-group-authentication\nname: Metamarkets RDI Authentication\ndescription: Authentication profile for the Metamarkets Real-time Data Ingestion (RDI) API.\ngenerated: '2026-07-20'\nmethod: searched\nsource: https://docs.metamarkets.com/docs/real-time-data-delivery\napi: Metamarkets Real-Time Data Ingestion (RDI) API\nschemes:\n- type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  description: >-\n    RDI endpoints are protected by HTTP Basic authentication. A per-customer\n    username and password are supplied by the Metamarkets data engineer / account\n    representative and passed on every POST (e.g. curl --user <username>:<password>).\n    HTTPS is required so credentials and data are always encrypted in transit.\n  credentialsProvisioning: manual\n  transport: https-required\nerrors:\n  invalidCredentials: >-\n    HTTP 401 is returned when credentials are incorrect or the caller lacks\n    permission to POST to the endpoint.\nnotes: >-\n\
  \  Endpoint URLs and credentials are provisioned per customer by a Metamarkets\n  data engineer; there is no self-service key issuance or OAuth flow documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metamarkets-group/refs/heads/main/authentication/metamarkets-group-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Advertising
- AdTech
- Analytics
- Programmatic Advertising
- Real-Time Data
- Data Ingestion
- OpenRTB
- Dashboards
---
