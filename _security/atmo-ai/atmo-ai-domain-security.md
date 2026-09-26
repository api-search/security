---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atmo.ai
  spf: false
hosts:
- cert_expires: Nov 28 21:59:32 2026 GMT
  host: www.atmo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atmo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmo AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Atmo AI
provider_slug: atmo-ai
slug: atmo-ai-domain-security
source_filename: atmo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atmo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 21:59:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atmo.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmo-ai/refs/heads/main/security/atmo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Weather
- AI
- Forecasting
- Climate
---
