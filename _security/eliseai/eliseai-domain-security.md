---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eliseai.com
  spf: true
hosts:
- cert_expires: Sep 29 04:03:22 2026 GMT
  host: www.eliseai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eliseai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EliseAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EliseAI
provider_slug: eliseai
slug: eliseai-domain-security
source_filename: eliseai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eliseai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:03:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eliseai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eliseai/refs/heads/main/security/eliseai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Property Management
- Real Estate
- Healthcare
- Leasing
- Voice AI
- Automation
- CRM
---
