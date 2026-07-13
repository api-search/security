---
api_specs:
- filename: Kroger-API-Spec-23c0b0b34f55c3d32d60fcb23de33a86.yaml
  format: yaml
  label: Kroger Product Catalog API
  slug: kroger-product-catalog-api
  spec_type: OpenAPI
  url: https://developer.kroger.com/assets/files/Kroger-API-Spec-23c0b0b34f55c3d32d60fcb23de33a86.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roundys.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kroger.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.roundys.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: developer.kroger.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roundys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roundy''s, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Roundy's
provider_slug: roundys
slug: roundys-domain-security
source_filename: roundys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roundys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\n- host: developer.kroger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: roundys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kroger.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roundys/refs/heads/main/security/roundys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Grocery
- Kroger
- Midwest
- Retail
- Supermarket
- Wisconsin
---
