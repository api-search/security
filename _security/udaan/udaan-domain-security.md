---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: udaan.com
  spf: true
hosts:
- cert_expires: Oct  3 16:47:11 2026 GMT
  host: udaan.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Udaan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Udaan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Udaan
provider_slug: udaan
slug: udaan-domain-security
source_filename: udaan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: udaan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:47:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: udaan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/udaan/refs/heads/main/security/udaan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketplace
- B2B
- eCommerce
- Wholesale
- Retail
- India
- Supply Chain
---
