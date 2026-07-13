---
api_specs:
- filename: tabit-openapi.yml
  format: yaml
  label: Tabit Orders API
  slug: tabit-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabit/refs/heads/main/openapi/tabit-openapi.yml
- filename: tabit-openapi.yml
  format: yaml
  label: Tabit Menu API
  slug: tabit-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabit/refs/heads/main/openapi/tabit-openapi.yml
- filename: tabit-openapi.yml
  format: yaml
  label: Tabit Reservations API
  slug: tabit-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabit/refs/heads/main/openapi/tabit-openapi.yml
- filename: tabit-openapi.yml
  format: yaml
  label: Tabit Payments API
  slug: tabit-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabit/refs/heads/main/openapi/tabit-openapi.yml
- filename: tabit-openapi.yml
  format: yaml
  label: Tabit Integrations API
  slug: tabit-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabit/refs/heads/main/openapi/tabit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tabit.cloud
  spf: true
hosts:
- cert_expires: Oct  9 14:51:16 2026 GMT
  host: www.tabit.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:45:00 2026 GMT
  host: support-us.tabit.cloud
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tabit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tabit
provider_slug: tabit
slug: tabit-domain-security
source_filename: tabit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tabit.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:51:16 2026 GMT\n  hsts: false\n- host: support-us.tabit.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:45:00 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: tabit.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabit/refs/heads/main/security/tabit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Point of Sale
- POS
- Hospitality
- Ordering
- Payments
---
