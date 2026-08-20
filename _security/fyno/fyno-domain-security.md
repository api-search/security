---
api_specs:
- filename: fyno-fire-an-event-api-openapi.yml
  format: yaml
  label: Fyno Fire an Event API
  slug: fyno-fire-an-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-fire-an-event-api-openapi.yml
- filename: fyno-fyno-verify-api-openapi.yml
  format: yaml
  label: Fyno Fyno Verify API
  slug: fyno-fyno-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-fyno-verify-api-openapi.yml
- filename: fyno-manage-user-profiles-api-openapi.yml
  format: yaml
  label: Fyno Manage User Profiles API
  slug: fyno-manage-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-manage-user-profiles-api-openapi.yml
- filename: fyno-manage-user-subscriptions-preferences-api-openapi.yml
  format: yaml
  label: Fyno Manage User Subscriptions & Preferences API
  slug: fyno-manage-user-subscriptions-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-manage-user-subscriptions-preferences-api-openapi.yml
- filename: fyno-suppression-list-api-openapi.yml
  format: yaml
  label: Fyno Suppression List API
  slug: fyno-suppression-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-suppression-list-api-openapi.yml
- filename: fyno-user-properties-api-openapi.yml
  format: yaml
  label: Fyno User Properties API
  slug: fyno-user-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-user-properties-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fyno.io
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: fyno.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api.fyno.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fyno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fyno, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Fyno
provider_slug: fyno
slug: fyno-domain-security
source_filename: fyno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fyno.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fyno.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fyno.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/security/fyno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Notification
- Messaging
- Communications
- Push Notifications
- Email
- SMS
- WhatsApp
- In-App
- Orchestration
- Multi-Channel
---
