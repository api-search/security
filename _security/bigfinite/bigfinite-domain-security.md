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
- cert_expires: Oct  1 05:50:38 2026 GMT
  host: aizon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bigfinite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigfinite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bigfinite
provider_slug: bigfinite
slug: bigfinite-domain-security
source_filename: bigfinite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aizon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:50:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aizon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigfinite/refs/heads/main/security/bigfinite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmaceutical Manufacturing
- Manufacturing Intelligence
- Artificial Intelligence
- Machine Learning
- GxP
- Life Sciences
- Data Platform
- Quality
- Batch Records
---
