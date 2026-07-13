---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hokudai.ac.jp
  spf: true
hosts:
- cert_expires: Dec 20 01:13:05 2026 GMT
  host: www.global.hokudai.ac.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 00:48:08 2026 GMT
  host: eprints.lib.hokudai.ac.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hokkaido Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hokkaido University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hokkaido University
provider_slug: hokkaido
slug: hokkaido-domain-security
source_filename: hokkaido-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.global.hokudai.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 01:13:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eprints.lib.hokudai.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hokudai.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hokkaido/refs/heads/main/security/hokkaido-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- Japan
---
