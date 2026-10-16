---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cfex.ai
  spf: true
hosts:
- cert_expires: Nov 27 06:18:23 2026 GMT
  host: cfex.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cfex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CFEX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CFEX
provider_slug: cfex
slug: cfex-domain-security
source_filename: cfex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cfex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 06:18:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cfex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfex/refs/heads/main/security/cfex-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Billing
- Settlement
- Energy
- Compute
- AI
- Token
- Enterprise
---
