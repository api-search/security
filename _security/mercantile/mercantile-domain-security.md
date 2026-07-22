---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getmercantile.com
  spf: true
hosts:
- cert_expires: Oct  2 07:45:33 2026 GMT
  host: www.getmercantile.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercantile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercantile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mercantile
provider_slug: mercantile
slug: mercantile-domain-security
source_filename: mercantile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmercantile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:45:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getmercantile.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercantile/refs/heads/main/security/mercantile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Credit Cards
- Card Issuing
- Embedded Finance
- Fintech
- Payments
- Loyalty and Rewards
- Affinity Programs
- Business Credit
- Mastercard
---
