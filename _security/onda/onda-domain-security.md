---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drinkonda.com
  spf: true
hosts:
- cert_expires: Oct  2 08:16:58 2026 GMT
  edge: cloudflare
  host: drinkonda.com
  hsts: true
  hsts_max_age: 7889238
  hsts_source: manual curl HEAD https://drinkonda.com/ 2026-08-26
  http_status: 404
  https: true
  origin_platform: Shopify
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Onda
provider_slug: onda
slug: onda-domain-security
source_filename: onda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py, plus a manual\n  curl HEAD to correct an HSTS false negative — see note)\nnote: >-\n  Onda publishes no API, so the only host in scope is the company's own storefront domain\n  drinkonda.com. The Shopify origin answers HTTP 404 \"This store is unavailable\" on every path\n  (checked 2026-08-26); the automated probe records hsts as null because its HEAD request raised\n  on that 404 before reading headers. A manual HEAD confirms the origin does send\n  Strict-Transport-Security: max-age=7889238, so hsts is recorded as true with the observed\n  max-age. Everything below is what was actually observed — an absent record (no CAA, no DNSSEC)\n  is valid data, not a gap in the probe.\nhosts:\n- host: drinkonda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:16:58 2026 GMT\n  http_status: 404\n  hsts: true\n  hsts_max_age: 7889238\n  hsts_source:\
  \ manual curl HEAD https://drinkonda.com/ 2026-08-26\n  edge: cloudflare\n  origin_platform: Shopify\ndomains:\n- domain: drinkonda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onda/refs/heads/main/security/onda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consumer Packaged Goods
- Beverages
- Alcohol
- Ready-to-Drink
- Tequila
- Direct-to-Consumer
- E-Commerce
- Retail
- Shopify
---
