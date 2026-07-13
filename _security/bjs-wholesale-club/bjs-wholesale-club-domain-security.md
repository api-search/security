---
api_specs:
- filename: bjs-wholesale-club-openapi.yaml
  format: yaml
  label: BJ's Wholesale Club API
  slug: bjs-wholesale-club
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/refs/heads/main/openapi/bjs-wholesale-club-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bjs.com
  spf: true
hosts:
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: www.bjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: api.bjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bjs Wholesale Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BJ''s Wholesale Club, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BJ's Wholesale Club
provider_slug: bjs-wholesale-club
slug: bjs-wholesale-club-domain-security
source_filename: bjs-wholesale-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: null\n- host: api.bjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bjs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/refs/heads/main/security/bjs-wholesale-club-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Ecommerce
- Membership
- Retail
- Wholesale
---
