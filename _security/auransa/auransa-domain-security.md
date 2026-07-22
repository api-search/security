---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: auransa.com
  spf: true
hosts:
- cert_expires: Oct  6 21:44:46 2026 GMT
  host: www.auransa.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auransa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auransa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Auransa
provider_slug: auransa
slug: auransa-domain-security
source_filename: auransa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auransa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:44:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: auransa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auransa/refs/heads/main/security/auransa-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Artificial Intelligence
- Machine Learning
- Oncology
- Life Sciences
- Healthcare
---
