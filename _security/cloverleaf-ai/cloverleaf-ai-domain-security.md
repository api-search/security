---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloverleaf.ai
  spf: true
hosts:
- cert_expires: Sep 28 05:34:48 2026 GMT
  host: www.cloverleaf.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloverleaf Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloverleaf AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cloverleaf AI
provider_slug: cloverleaf-ai
slug: cloverleaf-ai-domain-security
source_filename: cloverleaf-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloverleaf.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:34:48 2026 GMT\n  hsts: false\ndomains:\n- domain: cloverleaf.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloverleaf-ai/refs/heads/main/security/cloverleaf-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Government
- B2G
- Sales Intelligence
- Public Sector
- GovTech
- Procurement
- RFP
- Legislative Intelligence
- Speech to Text
- Artificial Intelligence
---
