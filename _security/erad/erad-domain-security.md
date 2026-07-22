---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: erad.co
  spf: true
hosts:
- cert_expires: Sep  7 20:45:20 2026 GMT
  host: erad.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Erad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Erad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Erad
provider_slug: erad
slug: erad-domain-security
source_filename: erad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: erad.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:45:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: erad.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erad/refs/heads/main/security/erad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial Services
- Lending
- SME Financing
- Working Capital
- Invoice Financing
- Embedded Finance
- Revenue Based Financing
- Saudi Arabia
- MENA
- Sharia Compliant
---
