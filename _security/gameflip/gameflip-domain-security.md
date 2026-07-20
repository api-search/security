---
api_specs:
- filename: gameflip-gfapi-openapi.yml
  format: yaml
  label: Gameflip API (GFAPI)
  slug: gameflip-api-gfapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameflip/refs/heads/main/openapi/gameflip-gfapi-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gameflip.com
  spf: true
- caa:
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: fingershock.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: gameflip.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: production-gameflip.fingershock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: test-gameflip.fingershock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gameflip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gameflip, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gameflip
provider_slug: gameflip
slug: gameflip-domain-security
source_filename: gameflip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gameflip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: production-gameflip.fingershock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: test-gameflip.fingershock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gameflip.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fingershock.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameflip/refs/heads/main/security/gameflip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Marketplace
- Digital Goods
- E-Commerce
- Payments
- Wallet
- Listings
- Steam
- Gift Cards
---
