---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tohoku.ac.jp
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nii.ac.jp
  spf: true
hosts:
- cert_expires: Mar 28 04:13:55 2027 GMT
  host: www.tohoku.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  3 09:14:11 2027 GMT
  host: tohoku.repo.nii.ac.jp
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tohoku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tohoku University, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tohoku University
provider_slug: tohoku
slug: tohoku-domain-security
source_filename: tohoku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tohoku.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 28 04:13:55 2027 GMT\n  hsts: false\n- host: tohoku.repo.nii.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 09:14:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: tohoku.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nii.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tohoku/refs/heads/main/security/tohoku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Japan
- Open Access
- Institutional Repository
- OAI-PMH
- Library
---
