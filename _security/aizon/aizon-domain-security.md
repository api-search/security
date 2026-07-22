---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aizon.ai
  spf: true
hosts:
- cert_expires: Sep 30 09:22:04 2026 GMT
  host: www.aizon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aizon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aizon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aizon
provider_slug: aizon
slug: aizon-domain-security
source_filename: aizon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aizon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aizon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aizon/refs/heads/main/security/aizon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmaceutical Manufacturing
- Life Sciences
- Artificial Intelligence
- Machine Learning
- Manufacturing Intelligence
- GxP
- Data Platform
- Quality
---
