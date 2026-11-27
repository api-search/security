---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Apidoor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apidoor declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Apidoor
provider_slug: apidoor
scheme_count: 3
schemes:
- description: Customers send the full Apidoor-issued key in the X-API-Key header to the project gateway hostname. Keys start with apdr_key_, are shown once, stored as a one-way hash, and cannot be retrieved, renamed, reassigned or rotated (revoke and replace).
  header: X-API-Key
  in: header
  key_prefix: apdr_key_
  name: ApiKeyHeader
  type: apiKey
- description: Apidoor adds the project verification secret to every forwarded request so the seller upstream can reject traffic that did not come through Apidoor. Cannot be recovered or rotated from the dashboard.
  direction: gateway-to-upstream
  header: x-apidoor-proxy-secret
  in: header
  name: UpstreamProxySecret
  type: apiKey
- description: 'Limit webhooks are signed: apidoor-signature has the form t=timestamp,v1=hex_signature, an HMAC-SHA256 of timestamp.raw_body with a signing secret starting apdr_whsec_.'
  direction: apidoor-to-seller
  header: apidoor-signature
  name: WebhookSignature
  type: hmac
slug: apidoor-authentication
source_filename: apidoor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource:\n- https://docs.apidoor.io/docs/send-requests\n- https://docs.apidoor.io/docs/api-keys\n- https://docs.apidoor.io/docs/projects-and-upstreams\n- https://docs.apidoor.io/docs/access-controls\ndocs: https://docs.apidoor.io/docs/send-requests\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  header: X-API-Key\n  description: Customers send the full Apidoor-issued key in the X-API-Key header to the project gateway hostname. Keys start\n    with apdr_key_, are shown once, stored as a one-way hash, and cannot be retrieved, renamed, reassigned or rotated (revoke\n    and replace).\n  key_prefix: apdr_key_\n- name: UpstreamProxySecret\n  type: apiKey\n  in: header\n  header: x-apidoor-proxy-secret\n  direction: gateway-to-upstream\n  description: Apidoor adds the project verification secret to every forwarded request so the seller upstream can reject traffic\n    that did not come through Apidoor. Cannot be recovered\
  \ or rotated from the dashboard.\n- name: WebhookSignature\n  type: hmac\n  header: apidoor-signature\n  direction: apidoor-to-seller\n  description: 'Limit webhooks are signed: apidoor-signature has the form t=timestamp,v1=hex_signature, an HMAC-SHA256 of\n    timestamp.raw_body with a signing secret starting apdr_whsec_.'\nnote: No OAuth. The seller dashboard (app.apidoor.io) is a browser sign-in, not a documented API.\n"
source_yaml_url: https://artifacts.apis.io/apidoor/authentication/apidoor-authentication.yml
summary_line: 3 schemes
tags:
- Company
- API Gateway
- API Monetization
- APIKeys
- Rate Limiting
- Usage Analytics
- API Subscriptions
- Billing
---
