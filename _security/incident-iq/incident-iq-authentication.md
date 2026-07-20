---
api_key_in: []
auth_types:
- http
- oauth1
description: ''
kind: authentication
layout: security
method: searched
name: Incident Iq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Incident IQ secures its APIs with http and oauth1 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Incident IQ
provider_slug: incident-iq
scheme_count: 4
schemes:
- description: 'Bearer token issued from Administration > Developer Tools. Sent on every request as `Authorization: Bearer <token>`.'
  in: header
  name: BearerToken
  parameter: Authorization
  scheme: bearer
  sources:
  - docs:https://apihub.incidentiq.com/
  type: http
- description: District/tenant site identifier (GUID) that scopes the request to a specific Incident IQ instance. Required on every request.
  in: header
  name: SiteId
  parameter: SiteId
  sources:
  - docs:https://apihub.incidentiq.com/
  type: apiKey
- description: Client type header; API integrations set this to the literal value `ApiClient`.
  in: header
  name: Client
  parameter: Client
  sources:
  - docs:https://apihub.incidentiq.com/
  type: apiKey
- description: OAuth 1.0 consumer key/secret provisioning used for select partner / identity-provider integrations (consumer key + secret + access token URL exchanged with Incident IQ). Not used for the general REST API.
  name: OAuth1Consumer
  sources:
  - docs:https://help.rapididentity.com/docs/integrating-rapididentity-with-incident-iq
  type: oauth1
slug: incident-iq-authentication
source_filename: incident-iq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apihub.incidentiq.com/\ndocs: https://www.incidentiq.com/platform/api\nsummary:\n  types:\n  - http\n  - oauth1\n  api_key_in: []\n  notes: >-\n    Incident IQ API requests are authenticated with a bearer token in the\n    Authorization header plus platform-scoping headers. The Authorization token,\n    SiteId, and Client credentials are issued from the Incident IQ\n    Administration > Developer Tools console. Some partner integrations (e.g.\n    identity providers) instead use OAuth 1.0 consumer key/secret provisioning.\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    Bearer token issued from Administration > Developer Tools. Sent on every\n    request as `Authorization: Bearer <token>`.\n  sources:\n  - docs:https://apihub.incidentiq.com/\n- name: SiteId\n  type: apiKey\n  in: header\n  parameter: SiteId\n  description: >-\n    District/tenant\
  \ site identifier (GUID) that scopes the request to a specific\n    Incident IQ instance. Required on every request.\n  sources:\n  - docs:https://apihub.incidentiq.com/\n- name: Client\n  type: apiKey\n  in: header\n  parameter: Client\n  description: >-\n    Client type header; API integrations set this to the literal value\n    `ApiClient`.\n  sources:\n  - docs:https://apihub.incidentiq.com/\n- name: OAuth1Consumer\n  type: oauth1\n  description: >-\n    OAuth 1.0 consumer key/secret provisioning used for select partner /\n    identity-provider integrations (consumer key + secret + access token URL\n    exchanged with Incident IQ). Not used for the general REST API.\n  sources:\n  - docs:https://help.rapididentity.com/docs/integrating-rapididentity-with-incident-iq\nrequired_headers:\n- SiteId\n- Authorization\n- Client\n- Content-Type\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incident-iq/refs/heads/main/authentication/incident-iq-authentication.yml
summary_line: http/oauth1 · 4 schemes
tags:
- Company
- Edtech
- IT Service Management
- Asset Management
- Help Desk
- Ticketing
- K-12
- Education
- Webhooks
- REST
---
