---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fgac.ai
  spf: true
hosts:
- cert_expires: Dec 15 19:26:55 2026 GMT
  host: fgac.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FGAC.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FGAC.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FGAC.ai
provider_slug: fgac-ai
slug: fgac-ai-domain-security
source_filename: fgac-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fgac.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 19:26:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fgac.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fgac-ai/security/fgac-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Security
- Access Control
- Proxy
- Platform
---
