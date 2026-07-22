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
- cert_expires: Oct  9 22:56:12 2026 GMT
  host: highalpha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: High Alpha Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for High Alpha Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: High Alpha Capital
provider_slug: high-alpha-capital
slug: high-alpha-capital-domain-security
source_filename: high-alpha-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 22:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: highalpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/high-alpha-capital/refs/heads/main/security/high-alpha-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venture Capital
- Venture Studio
- B2B SaaS
- Enterprise Software
- Startups
- Investment
---
