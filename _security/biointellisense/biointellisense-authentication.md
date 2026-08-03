---
api_key_in: []
auth_types:
- unknown-bearer
description: ''
kind: authentication
layout: security
method: probed
name: Biointellisense Authentication
name_suffix: Authentication
oauth_flows: []
overview: BioIntelliSense secures its APIs with unknown-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BioIntelliSense
provider_slug: biointellisense
scheme_count: 1
schemes:
- confidence: medium
  description: Every path on the BioCloud API host rejects anonymous requests with HTTP 401 and the JSON body {"code":"authentication_header_missing","description":"Authentication header is expected"}. The gate therefore requires an Authorization request header, but the credential type (bearer JWT, opaque token, API key) is not disclosed anonymously and BioIntelliSense publishes no developer authentication documentation.
  in: header
  name: authorization-header
  parameter: Authorization
  scheme: unknown
  sources:
  - probe://biocloud.biointellisense.com
  type: http
slug: biointellisense-authentication
source_filename: biointellisense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live probe of https://biocloud.biointellisense.com (no OpenAPI available to derive from)\nsummary:\n  types: [unknown-bearer]\n  api_key_in: []\n  oauth2_flows: []\n  public_docs: false\n  self_service_signup: false\nschemes:\n- name: authorization-header\n  type: http\n  scheme: unknown\n  in: header\n  parameter: Authorization\n  description: 'Every path on the BioCloud API host rejects anonymous requests with\n    HTTP 401 and the JSON body {\"code\":\"authentication_header_missing\",\"description\":\"Authentication\n    header is expected\"}. The gate therefore requires an Authorization request header,\n    but the credential type (bearer JWT, opaque token, API key) is not disclosed anonymously\n    and BioIntelliSense publishes no developer authentication documentation.'\n  sources: [probe://biocloud.biointellisense.com]\n  confidence: medium\nobservations:\n- host: biocloud.biointellisense.com\n  http_status: 401\n  content_type:\
  \ application/json\n  body: '{\"code\":\"authentication_header_missing\",\"description\":\"Authentication header\n    is expected\"}'\n  server: gunicorn\n  fronted_by: biocloud-internal-api-alb (AWS ELB, us-east-2)\n- host: data.biointellisense.com\n  note: 'TLS terminates (Google Cloud LB, 34.96.68.71, cert verifies) but the host\n    returns no HTTP response to an anonymous HTTP/1.1 or HTTP/2 request and rejects\n    standard TLS clients — consistent with a mutual-TLS or client-certificate-gated\n    device-ingest endpoint. Not confirmed.'\n- host: api.biointellisense.com\n  note: 'DANGLING CNAME. api.biointellisense.com -> demo19-prod.apigee.net, which has\n    no A record on Google (8.8.8.8) or Cloudflare (1.1.1.1) resolvers as of 2026-08-02.\n    The Apigee organization it pointed at appears decommissioned; the DNS record was\n    not withdrawn. This is a stale record, not a live API host, and is a subdomain-takeover\n    exposure worth flagging to the provider.'\ndiscovery:\n  oauth_metadata:\
  \ none (401 on /.well-known/oauth-authorization-server)\n  openid_configuration: none (401 on /.well-known/openid-configuration)\n  docs: null\nx-evidence:\n  fetched: '2026-08-02'\n  paths_probed: 19\n  anonymous_200s: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biointellisense/refs/heads/main/authentication/biointellisense-authentication.yml
summary_line: unknown-bearer · 1 scheme
tags:
- Company
- Health
- Healthcare
- Remote Patient Monitoring
- Wearables
- Medical Devices
- Vital Signs
- Continuous Monitoring
- Digital Health
- Data as a Service
---
