---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 1910.ai
  spf: true
hosts:
- cert_expires: Oct  6 19:55:36 2026 GMT
  host: www.1910.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1910 Genetics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1910 Genetics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 1910 Genetics
provider_slug: 1910-genetics
slug: 1910-genetics-domain-security
source_filename: 1910-genetics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1910.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:55:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1910.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1910-genetics/refs/heads/main/security/1910-genetics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Engineered Biology
- Drug Discovery
- Artificial Intelligence
- Biotechnology
- Machine Learning
- Life Sciences
- Laboratory Automation
---
