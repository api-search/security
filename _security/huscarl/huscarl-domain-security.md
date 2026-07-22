---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: huscarl.io
  spf: true
hosts:
- cert_expires: Sep  6 06:36:48 2026 GMT
  host: www.huscarl.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Huscarl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huscarl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Huscarl
provider_slug: huscarl
slug: huscarl-domain-security
source_filename: huscarl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huscarl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:36:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: huscarl.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huscarl/refs/heads/main/security/huscarl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Actuarial
- Captive Insurance
- Self-Insurance
- Risk Management
- Underwriting
- Y Combinator
- Artificial Intelligence
---
