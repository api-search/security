---
api_specs:
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Booking API
  slug: booking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Rate Plan API
  slug: rateplan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Finance API
  slug: finance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Settings API
  slug: settings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Webhook API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apaleo.com
  spf: true
hosts:
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: www.apaleo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: api.apaleo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: webhook.apaleo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Apaleo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apaleo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: apaleo
provider_slug: apaleo
slug: apaleo-domain-security
source_filename: apaleo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apaleo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.apaleo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: webhook.apaleo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: apaleo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/security/apaleo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Hospitality
- PMS
- Property Management
- Hotels
- API-First
---
