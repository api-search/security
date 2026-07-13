---
api_specs:
- filename: spothero-parking-openapi.yml
  format: yaml
  label: SpotHero Parking API
  slug: spothero-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spothero/refs/heads/main/openapi/spothero-parking-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spothero.com
  spf: true
hosts:
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: spothero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: api.spothero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spothero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpotHero, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SpotHero
provider_slug: spothero
slug: spothero-domain-security
source_filename: spothero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spothero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: false\n- host: api.spothero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spothero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spothero/refs/heads/main/security/spothero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Parking
- Mobility
- Transportation
- Navigation
- Reservations
---
