---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: otago.ac.nz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reannz.co.nz
  spf: true
hosts:
- cert_expires: Sep 21 04:35:44 2026 GMT
  host: www.otago.ac.nz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 01:09:10 2026 GMT
  host: ourarchive.otago.ac.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 07:05:33 2026 GMT
  host: www.reannz.co.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Otago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Otago, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Otago
provider_slug: university-of-otago
slug: university-of-otago-domain-security
source_filename: university-of-otago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.otago.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 04:35:44 2026 GMT\n  hsts: null\n- host: ourarchive.otago.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:09:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.reannz.co.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 07:05:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: otago.ac.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: reannz.co.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-otago/refs/heads/main/security/university-of-otago-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Identity
- New Zealand
---
