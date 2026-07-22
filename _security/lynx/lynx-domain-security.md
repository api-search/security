---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lynx-fh.com
  spf: true
hosts:
- cert_expires: Sep 19 10:39:41 2026 GMT
  host: lynx-fh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lynx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lynx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lynx
provider_slug: lynx
slug: lynx-domain-security
source_filename: lynx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lynx-fh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 10:39:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lynx-fh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lynx/refs/heads/main/security/lynx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Fintech
- Payments
- Benefits
- Health Savings Accounts
- Embedded Finance
- Card Issuing
- Insurance
---
