---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moneyboxapp.com
  spf: true
hosts:
- cert_expires: Oct 12 04:40:14 2026 GMT
  host: www.moneyboxapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moneybox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moneybox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Moneybox
provider_slug: moneybox
slug: moneybox-domain-security
source_filename: moneybox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moneyboxapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:40:14 2026 GMT\n  hsts: null\ndomains:\n- domain: moneyboxapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneybox/refs/heads/main/security/moneybox-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Financial-Services
- Fintech
- Wealth Management
- Savings
- Investing
- Pensions
- Open Banking
- Consumer Finance
- Mobile Apps
- United Kingdom
---
