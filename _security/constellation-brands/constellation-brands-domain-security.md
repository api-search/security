---
api_specs:
- filename: constellation-brands-openapi.yml
  format: yaml
  label: Product Items API
  slug: product
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "zerossl.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cbrands.com
  spf: true
hosts:
- cert_expires: Sep  8 23:04:04 2026 GMT
  host: www.cbrands.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 06:49:16 2026 GMT
  host: dev.cbrands.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.cbrands.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Constellation Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constellation Brands, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Constellation Brands
provider_slug: constellation-brands
slug: constellation-brands-domain-security
source_filename: constellation-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:04:04 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: dev.cbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:49:16 2026 GMT\n  hsts: false\n- host: api.cbrands.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cbrands.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"zerossl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/security/constellation-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alcohol
- Beer
- Beverages
- Digital Assets
- Fortune 500
- Spirits
- Wine
---
