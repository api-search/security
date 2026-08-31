---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ten63tx.com
  spf: true
hosts:
- cert_expires: Nov  2 08:38:18 2026 GMT
  host: www.ten63tx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ten63 Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ten63 Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Ten63 Therapeutics
provider_slug: ten63-therapeutics
slug: ten63-therapeutics-domain-security
source_filename: ten63-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ten63tx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:38:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ten63tx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ten63-therapeutics/refs/heads/main/security/ten63-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Artificial Intelligence
- Machine-Learning
- Computational Chemistry
- Oncology
- Life Sciences
- Research
---
