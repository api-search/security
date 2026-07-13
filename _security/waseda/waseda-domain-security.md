---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: waseda.jp
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nii.ac.jp
  spf: true
hosts:
- cert_expires: Aug 19 22:11:59 2026 GMT
  host: www.waseda.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  3 09:33:58 2027 GMT
  host: waseda.repo.nii.ac.jp
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: waseda.primo.exlibrisgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waseda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waseda University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Waseda University
provider_slug: waseda
slug: waseda-domain-security
source_filename: waseda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.waseda.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 22:11:59 2026 GMT\n  hsts: false\n- host: waseda.repo.nii.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 09:33:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: waseda.primo.exlibrisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: waseda.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nii.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waseda/refs/heads/main/security/waseda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Access
- Japan
---
