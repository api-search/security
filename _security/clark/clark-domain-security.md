---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clark.de
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.clark.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clark
provider_slug: clark
slug: clark-domain-security
source_filename: clark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clark.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clark.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clark/refs/heads/main/security/clark-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Insurance Comparison
- Personal Finance
- Financial Services
- Consumer
- Germany
- Mobile App
---
