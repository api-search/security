---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unlearn.ai
  spf: true
hosts:
- cert_expires: Aug 25 00:24:03 2026 GMT
  host: unlearn.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unlearn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unlearn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unlearn
provider_slug: unlearn
slug: unlearn-domain-security
source_filename: unlearn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unlearn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:24:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unlearn.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unlearn/refs/heads/main/security/unlearn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotech
- Artificial Intelligence
- Clinical Trials
- Digital Twins
- Machine Learning
- Healthcare
---
