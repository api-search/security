---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eyva.ai
  spf: true
hosts:
- cert_expires: Sep 16 14:22:20 2026 GMT
  host: www.eyva.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eyva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eyva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eyva
provider_slug: eyva
slug: eyva-domain-security
source_filename: eyva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eyva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:22:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eyva.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eyva/refs/heads/main/security/eyva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beauty
- Personal Care
- Consumer Insights
- Market Intelligence
- Artificial Intelligence
- Product Development
- Trend Detection
- SaaS
- Analytics
---
