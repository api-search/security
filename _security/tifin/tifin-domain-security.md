---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tifin.com
  spf: true
hosts:
- cert_expires: Nov 27 14:42:05 2026 GMT
  host: tifin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tifin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TIFIN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TIFIN
provider_slug: tifin
slug: tifin-domain-security
source_filename: tifin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tifin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 14:42:05 2026 GMT\n  hsts: false\ndomains:\n- domain: tifin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tifin/refs/heads/main/security/tifin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial-Services
- Wealth Management
- Asset Management
- Artificial Intelligence
- Fintech
- WealthTech
- Financial Advisors
- Investment Management
- Insurance
---
