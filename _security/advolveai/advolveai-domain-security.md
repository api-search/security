---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: advolve.ai
  spf: true
hosts:
- cert_expires: Aug 29 05:45:11 2026 GMT
  host: advolve.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Advolveai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advolve.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Advolve.AI
provider_slug: advolveai
slug: advolveai-domain-security
source_filename: advolveai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: advolve.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:45:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: advolve.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advolveai/refs/heads/main/security/advolveai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Advertising
- Marketing
- AdTech
- MarTech
- Performance Marketing
- E-commerce
- Brazil
---
