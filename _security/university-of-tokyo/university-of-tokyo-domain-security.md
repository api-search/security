---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: u-tokyo.ac.jp
  spf: true
hosts:
- cert_expires: Dec  6 03:13:04 2026 GMT
  host: www.u-tokyo.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 10 14:53:50 2026 GMT
  host: da.dl.itc.u-tokyo.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 30 02:08:06 2027 GMT
  host: repository.dl.itc.u-tokyo.ac.jp
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Tokyo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Tokyo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Tokyo
provider_slug: university-of-tokyo
slug: university-of-tokyo-domain-security
source_filename: university-of-tokyo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.u-tokyo.ac.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 03:13:04 2026 GMT\n  hsts: false\n- host: da.dl.itc.u-tokyo.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 14:53:50 2026 GMT\n  hsts: false\n- host: repository.dl.itc.u-tokyo.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 02:08:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: u-tokyo.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/security/university-of-tokyo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Japan
- Research
- Library
- Digital Archives
- IIIF
- Open Data
- OAI-PMH
---
