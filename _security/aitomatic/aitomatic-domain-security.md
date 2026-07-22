---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aitomatic.com
  spf: true
hosts:
- cert_expires: Oct  4 10:32:08 2026 GMT
  host: www.aitomatic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aitomatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aitomatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aitomatic
provider_slug: aitomatic
slug: aitomatic-domain-security
source_filename: aitomatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aitomatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:32:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aitomatic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aitomatic/refs/heads/main/security/aitomatic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- Industrial AI
- Neurosymbolic
- Semiconductor
- Open Source
- Machine Learning
---
