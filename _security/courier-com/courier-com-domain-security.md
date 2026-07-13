---
api_specs:
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Send API
  slug: courier-com-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Messages API
  slug: courier-com-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Lists API
  slug: courier-com-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier User Profiles API
  slug: courier-com-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier User Preferences API
  slug: courier-com-user-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Device Tokens API
  slug: courier-com-device-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Notification Templates API
  slug: courier-com-notification-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Brands API
  slug: courier-com-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Automations API
  slug: courier-com-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Audiences API
  slug: courier-com-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Tenants API
  slug: courier-com-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Bulk API
  slug: courier-com-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Audit Events API
  slug: courier-com-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Translations API
  slug: courier-com-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: courier.com
  spf: true
hosts:
- cert_expires: Oct  4 22:32:39 2026 GMT
  host: www.courier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 13:36:56 2026 GMT
  host: api.courier.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Courier Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Courier, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Courier
provider_slug: courier-com
slug: courier-com-domain-security
source_filename: courier-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.courier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:32:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.courier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:36:56 2026 GMT\n  hsts: null\ndomains:\n- domain: courier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/security/courier-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notifications
- Messaging
- Email
- SMS
- Push
- Multi-Channel
- Notification Infrastructure
- In-App Inbox
---
