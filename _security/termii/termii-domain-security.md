---
api_specs:
- filename: termii-campaigns-api-openapi.yml
  format: yaml
  label: Termii Campaigns API
  slug: termii-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-campaigns-api-openapi.yml
- filename: termii-contacts-api-openapi.yml
  format: yaml
  label: Termii Contacts API
  slug: termii-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-contacts-api-openapi.yml
- filename: termii-insights-api-openapi.yml
  format: yaml
  label: Termii Insights API
  slug: termii-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-insights-api-openapi.yml
- filename: termii-messaging-api-openapi.yml
  format: yaml
  label: Termii Messaging API
  slug: termii-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-messaging-api-openapi.yml
- filename: termii-sender-ids-api-openapi.yml
  format: yaml
  label: Termii Sender IDs API
  slug: termii-sender-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-sender-ids-api-openapi.yml
- filename: termii-token-api-openapi.yml
  format: yaml
  label: Termii Token API
  slug: termii-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: termii.com
  spf: true
hosts:
- cert_expires: Sep 23 09:44:30 2026 GMT
  host: termii.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:00:10 2026 GMT
  host: developers.termii.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 07:44:32 2026 GMT
  host: api.ng.termii.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Termii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Termii, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Termii
provider_slug: termii
slug: termii-domain-security
source_filename: termii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: termii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:44:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.termii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ng.termii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:44:32 2026 GMT\n  hsts: null\ndomains:\n- domain: termii.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/security/termii-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- SMS
- OTP
- WhatsApp
- Verification
---
