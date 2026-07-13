---
api_specs:
- filename: quandoo-public-partner-api-openapi.yml
  format: yaml
  label: Quandoo Public Partner API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-public-partner-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quandoo.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.quandoo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: docs.quandoo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: public-api.prod.quandoo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Quandoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quandoo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quandoo
provider_slug: quandoo
slug: quandoo-domain-security
source_filename: quandoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quandoo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.quandoo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\n- host: public-api.prod.quandoo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: quandoo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/security/quandoo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Restaurant
- Reservations
- Booking
- Availability
- Merchants
- Marketplace
---
