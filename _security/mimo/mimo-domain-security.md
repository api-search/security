---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mimohq.com
  spf: true
hosts:
- cert_expires: Sep 14 16:25:52 2026 GMT
  host: www.mimohq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mimo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mimo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mimo
provider_slug: mimo
slug: mimo-domain-security
source_filename: mimo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mimohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:25:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mimohq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mimo/refs/heads/main/security/mimo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Cash Flow Management
- Accounting
- Bookkeeping
- SMB
- B2B
---
