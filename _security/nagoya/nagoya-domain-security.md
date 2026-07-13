---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nagoya-u.ac.jp
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nii.ac.jp
  spf: true
hosts:
- cert_expires: Apr  5 07:48:17 2027 GMT
  host: en.nagoya-u.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 04:28:36 2026 GMT
  host: nagoya.repo.nii.ac.jp
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nagoya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nagoya University, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nagoya University
provider_slug: nagoya
slug: nagoya-domain-security
source_filename: nagoya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.nagoya-u.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 07:48:17 2027 GMT\n  hsts: false\n- host: nagoya.repo.nii.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 04:28:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: nagoya-u.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nii.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nagoya/refs/heads/main/security/nagoya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- OAI-PMH
- Japan
---
