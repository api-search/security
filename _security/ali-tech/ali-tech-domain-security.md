---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xaim.io
  spf: true
hosts:
- cert_expires: Oct 14 03:01:07 2026 GMT
  host: xaim.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ali Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ali Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ali Tech
provider_slug: ali-tech
slug: ali-tech-domain-security
source_filename: ali-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xaim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 03:01:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xaim.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ali-tech/refs/heads/main/security/ali-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- AI Infrastructure
- Compute
- Machine Learning
- Cost Optimization
- APIs
---
