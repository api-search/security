---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: otocapital.in
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: otocapital.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Oto Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oto Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oto Capital
provider_slug: oto-capital
slug: oto-capital-domain-security
source_filename: oto-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otocapital.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: otocapital.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oto-capital/refs/heads/main/security/oto-capital-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Two-Wheeler
- Financing
- Fintech
- Lending
- Consumer Finance
- Mobility
- E-Commerce
- India
---
