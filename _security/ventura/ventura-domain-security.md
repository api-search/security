---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ventura.ai
  spf: true
hosts:
- cert_expires: Oct  2 02:53:37 2026 GMT
  host: www.ventura.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ventura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ventura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ventura
provider_slug: ventura
slug: ventura-domain-security
source_filename: ventura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ventura.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:53:37 2026 GMT\n  hsts: false\ndomains:\n- domain: ventura.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ventura/refs/heads/main/security/ventura-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Distributors
- Manufacturers
- Quoting
- Order Entry
- ERP
- Industrials
- Sales Automation
- Y Combinator
---
