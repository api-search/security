---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: farther.com
  spf: true
hosts:
- cert_expires: Oct  9 16:21:23 2026 GMT
  host: www.farther.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farther Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farther, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Farther
provider_slug: farther
slug: farther-domain-security
source_filename: farther-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.farther.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:21:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: farther.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farther/refs/heads/main/security/farther-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Wealth Management
- Financial Services
- Registered Investment Advisor
- Financial Planning
- Investment Management
- WealthTech
---
