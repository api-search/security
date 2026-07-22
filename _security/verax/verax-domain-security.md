---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: verax.ai
  spf: true
hosts:
- cert_expires: Oct 14 21:59:38 2026 GMT
  host: verax.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Verax
provider_slug: verax
slug: verax-domain-security
source_filename: verax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verax.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:59:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verax.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verax/refs/heads/main/security/verax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Security
- AI Governance
- Generative AI
- Data Loss Prevention
- Shadow AI
- LLM
- Enterprise Security
---
