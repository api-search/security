---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lattica.ai
  spf: true
hosts:
- cert_expires: Oct 10 15:02:34 2026 GMT
  host: www.lattica.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 21:40:11 2026 GMT
  host: platformdocs.lattica.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.lattica.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lattica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lattica, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lattica
provider_slug: lattica
slug: lattica-domain-security
source_filename: lattica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lattica.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 15:02:34 2026 GMT\n  hsts: false\n- host: platformdocs.lattica.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:40:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lattica.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lattica.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lattica/refs/heads/main/security/lattica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Privacy
- Fully Homomorphic Encryption
- Encryption
- Confidential Computing
- Artificial Intelligence
- Machine Learning
- Inference
- Vector Search
- Security
---
