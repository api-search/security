---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fama.io
  spf: true
hosts:
- cert_expires: Oct 15 18:46:54 2026 GMT
  host: fama.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fama
provider_slug: fama
slug: fama-domain-security
source_filename: fama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fama.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:46:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fama.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fama/refs/heads/main/security/fama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employment Screening
- Background Checks
- Human Resources
- Social Media
- Risk
- Compliance
- Artificial Intelligence
---
