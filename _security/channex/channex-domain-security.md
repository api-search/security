---
api_specs:
- filename: channex-openapi.yml
  format: yaml
  label: Channex Properties API
  slug: properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-openapi.yml
- filename: channex-openapi.yml
  format: yaml
  label: Channex Room Types API
  slug: room-types
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-openapi.yml
- filename: channex-openapi.yml
  format: yaml
  label: Channex Rate Plans API
  slug: rate-plans
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-openapi.yml
- filename: channex-openapi.yml
  format: yaml
  label: Channex Availability and Restrictions (ARI) API
  slug: availability-restrictions-ari
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-openapi.yml
- filename: channex-openapi.yml
  format: yaml
  label: Channex Bookings API
  slug: bookings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-openapi.yml
- filename: channex-openapi.yml
  format: yaml
  label: Channex Channels API
  slug: channels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-openapi.yml
- filename: channex-openapi.yml
  format: yaml
  label: Channex Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/openapi/channex-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: channex.io
  spf: true
hosts:
- cert_expires: Sep 29 18:54:21 2026 GMT
  host: channex.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 07:01:31 2026 GMT
  host: docs.channex.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: secure.channex.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Channex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Channex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Channex
provider_slug: channex
slug: channex-domain-security
source_filename: channex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: channex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:54:21 2026 GMT\n  hsts: false\n- host: docs.channex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 07:01:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.channex.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: channex.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channex/refs/heads/main/security/channex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- Channel Manager
- Hotel Distribution
- OTA
- Bookings
---
