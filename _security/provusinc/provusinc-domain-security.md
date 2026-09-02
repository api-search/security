---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: provus.ai
  spf: true
hosts:
- cert_expires: Oct 17 21:44:07 2026 GMT
  host: provus.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Provusinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Provus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Provus
provider_slug: provusinc
slug: provusinc-domain-security
source_filename: provusinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: provus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:44:07 2026 GMT\n  hsts: false\ndomains:\n- domain: provus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provusinc/refs/heads/main/security/provusinc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- CPQ
- Services Quoting
- Professional Services
- Pricing
- AI Agents
- Sales
- Software-as-a-Service
---
