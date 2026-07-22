---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: earth-ai.com
  spf: false
hosts:
- cert_expires: Oct  4 10:33:47 2026 GMT
  host: www.earth-ai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earth Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earth AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Earth AI
provider_slug: earth-ai
slug: earth-ai-domain-security
source_filename: earth-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.earth-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: earth-ai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earth-ai/refs/heads/main/security/earth-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Critical Minerals
- Mineral Exploration
- Mining
- Geospatial
- Geoscience
- Machine Learning
- Natural Resources
- Climate Tech
---
