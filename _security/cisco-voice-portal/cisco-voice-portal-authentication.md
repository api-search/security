---
api_key_in:
- cookie
api_specs:
- filename: cisco-voice-portal-call-control-openapi.yml
  format: yaml
  label: Cisco Voice Portal Call Control API
  slug: cisco-voice-portal-call-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/openapi/cisco-voice-portal-call-control-openapi.yml
- filename: cisco-voice-portal-reporting-openapi.yml
  format: yaml
  label: Cisco Voice Portal Reporting API
  slug: cisco-voice-portal-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/openapi/cisco-voice-portal-reporting-openapi.yml
- filename: cisco-voice-portal-administration-openapi.yml
  format: yaml
  label: Cisco Voice Portal Administration API
  slug: cisco-voice-portal-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/openapi/cisco-voice-portal-administration-openapi.yml
- filename: cisco-voice-portal-vxml-services-openapi.yml
  format: yaml
  label: Cisco Voice Portal VXML Services API
  slug: cisco-voice-portal-vxml-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/openapi/cisco-voice-portal-vxml-services-openapi.yml
- filename: cisco-voice-portal-call-events-asyncapi.yml
  format: yaml
  label: Cisco Voice Portal Call Events API
  slug: cisco-voice-portal-call-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/asyncapi/cisco-voice-portal-call-events-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Voice Portal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Voice Portal secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
scheme_count: 2
schemes:
- description: HTTP Basic authentication using CVP OAMP administrative credentials. The default administrator account is configured during CVP installation.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cisco-voice-portal-administration-openapi.yml
  - openapi/cisco-voice-portal-call-control-openapi.yml
  - openapi/cisco-voice-portal-reporting-openapi.yml
  - openapi/cisco-voice-portal-vxml-services-openapi.yml
  type: http
- description: Session-based authentication obtained after login. The JSESSIONID cookie is returned after successful basic authentication.
  in: cookie
  name: sessionCookie
  parameter: JSESSIONID
  sources:
  - openapi/cisco-voice-portal-administration-openapi.yml
  type: apiKey
slug: cisco-voice-portal-authentication
source_filename: cisco-voice-portal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-voice-portal-administration-openapi.yml, openapi/cisco-voice-portal-call-control-openapi.yml,\n  openapi/cisco-voice-portal-reporting-openapi.yml, openapi/cisco-voice-portal-vxml-services-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using CVP OAMP administrative credentials. The default\n    administrator account is configured during CVP installation.\n  sources:\n  - openapi/cisco-voice-portal-administration-openapi.yml\n  - openapi/cisco-voice-portal-call-control-openapi.yml\n  - openapi/cisco-voice-portal-reporting-openapi.yml\n  - openapi/cisco-voice-portal-vxml-services-openapi.yml\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  description: Session-based authentication obtained after login. The JSESSIONID cookie is returned\n    after successful\
  \ basic authentication.\n  sources:\n  - openapi/cisco-voice-portal-administration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/authentication/cisco-voice-portal-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
---
