---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Signalfx Authentication
name_suffix: Authentication
oauth_flows: []
overview: SignalFx secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SignalFx
provider_slug: signalfx
scheme_count: 1
schemes:
- applies_to:
  - host: ingest.{realm}.signalfx.com
    plane: ingest
    token: org/ingest access token
  - host: api.{realm}.signalfx.com
    plane: rest
    token: API/session token
  - host: stream.{realm}.signalfx.com
    plane: signalflow
    token: access token
  description: 'Token passed in the X-SF-Token header. Three token classes exist: an organization (ingest) access token for the data-ingest API, a user/API (session) token for the REST metadata/config API, and an access token for the SignalFlow streaming API.'
  in: header
  name: XSFToken
  parameter_name: X-SF-Token
  type: apiKey
slug: signalfx-authentication
source_filename: signalfx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://dev.splunk.com/observability/docs/apibasics/authentication_org_tokens/\ndocs: https://dev.splunk.com/observability/docs/apibasics/authentication_org_tokens/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    SignalFx / Splunk Observability Cloud authenticates all API traffic with a\n    token supplied in the X-SF-Token request header. There are distinct token\n    classes for distinct API planes.\nschemes:\n- name: XSFToken\n  type: apiKey\n  in: header\n  parameter_name: X-SF-Token\n  description: >-\n    Token passed in the X-SF-Token header. Three token classes exist: an\n    organization (ingest) access token for the data-ingest API, a user/API\n    (session) token for the REST metadata/config API, and an access token for\n    the SignalFlow streaming API.\n  applies_to:\n  - plane: ingest\n    host: ingest.{realm}.signalfx.com\n    token: org/ingest access token\n  - plane:\
  \ rest\n    host: api.{realm}.signalfx.com\n    token: API/session token\n  - plane: signalflow\n    host: stream.{realm}.signalfx.com\n    token: access token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signalfx/refs/heads/main/authentication/signalfx-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Observability
- Monitoring
- Metrics
- Time Series
- APM
- Infrastructure Monitoring
- Alerting
- DevOps
- Splunk
---
