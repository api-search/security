---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: claros.tech
  spf: true
hosts:
- cert_expires: Oct  5 14:17:17 2026 GMT
  host: claros.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Claros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claros, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Claros
provider_slug: claros
slug: claros-domain-security
source_filename: claros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claros.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:17:17 2026 GMT\n  hsts: false\ndomains:\n- domain: claros.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claros/refs/heads/main/security/claros-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Center
- Power Management
- Energy Efficiency
- AI Infrastructure
- Hardware
- Semiconductors
- Sustainability
---
