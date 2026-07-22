---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: highalpha.com
  spf: true
hosts:
- cert_expires: Oct  9 19:40:47 2026 GMT
  host: www.highalpha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: High Alpha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for High Alpha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: High Alpha
provider_slug: high-alpha
slug: high-alpha-domain-security
source_filename: high-alpha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.highalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 19:40:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: highalpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/high-alpha/refs/heads/main/security/high-alpha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venture Studio
- Venture Capital
- B2B SaaS
- Startups
- Investment
- Enterprise Software
- Indianapolis
---
