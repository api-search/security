---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: provusinc.com
  spf: true
hosts:
- cert_expires: Oct  3 04:28:45 2026 GMT
  host: provusinc.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Provusinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Provus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Provus
provider_slug: provusinc
slug: provusinc-domain-security
source_filename: provusinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: provusinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:28:45 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: provusinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provusinc/refs/heads/main/security/provusinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CPQ
- Configure Price Quote
- Services Quoting
- Professional Services
- Pricing
- AI Agents
- Sales
- SaaS
---
