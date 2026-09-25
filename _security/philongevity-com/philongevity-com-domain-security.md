---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: philongevity.com
  spf: true
hosts:
- cert_expires: Dec 11 16:33:19 2026 GMT
  host: philongevity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Philongevity Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phi Longevity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Phi Longevity
provider_slug: philongevity-com
slug: philongevity-com-domain-security
source_filename: philongevity-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: philongevity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 16:33:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: philongevity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philongevity-com/refs/heads/main/security/philongevity-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Data
- Lab Results
- Biomarkers
- Chronic Disease
- Longevity
- MCP
- A2A
- Agentic Payments
- x402
- Artificial Intelligence
---
