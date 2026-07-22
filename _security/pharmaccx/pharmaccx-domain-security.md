---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ccx.tech
  spf: true
hosts:
- cert_expires: Oct  3 05:28:23 2026 GMT
  host: www.ccx.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pharmaccx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PharmaCCX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: PharmaCCX
provider_slug: pharmaccx
slug: pharmaccx-domain-security
source_filename: pharmaccx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ccx.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:28:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ccx.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pharmaccx/refs/heads/main/security/pharmaccx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Healthcare
- Pharmaceutical
- Market Access
- Pricing
- Contract Management
- Payers
- Enterprise SaaS
---
