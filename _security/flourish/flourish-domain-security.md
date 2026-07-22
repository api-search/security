---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flourishlabs.ai
  spf: true
hosts:
- cert_expires: Sep  3 20:33:50 2026 GMT
  host: www.flourishlabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flourish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flourish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flourish
provider_slug: flourish
slug: flourish-domain-security
source_filename: flourish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flourishlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flourishlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flourish/refs/heads/main/security/flourish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Machine Learning
- Research
- AI Research Lab
- New York
---
