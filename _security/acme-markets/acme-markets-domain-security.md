---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acmemarkets.com
  spf: true
hosts:
- cert_expires: Sep  9 22:57:06 2026 GMT
  host: www.acmemarkets.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:45:42 2026 GMT
  host: local.acmemarkets.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acme Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acme Markets, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Acme Markets
provider_slug: acme-markets
slug: acme-markets-domain-security
source_filename: acme-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acmemarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:57:06 2026 GMT\n  hsts: false\n- host: local.acmemarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:45:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acmemarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acme-markets/refs/heads/main/security/acme-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Albertsons Banner
- Delivery
- E-Commerce
- Grocery
- Loyalty
- Pharmacy
- Retail
- Store Locator
- Supermarket
---
