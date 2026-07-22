---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepmind.google
  spf: true
hosts:
- cert_expires: Sep 26 03:45:13 2026 GMT
  host: deepmind.google
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepmind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepMind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DeepMind
provider_slug: deepmind
slug: deepmind-domain-security
source_filename: deepmind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepmind.google\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:45:13 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: deepmind.google\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepmind/refs/heads/main/security/deepmind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Machine Learning
- Foundation Models
- LLMs
- Research
- Robotics
- Developer Tools
---
