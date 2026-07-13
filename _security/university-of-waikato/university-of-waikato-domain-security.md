---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: waikato.ac.nz
  spf: true
hosts:
- cert_expires: Aug 23 11:09:55 2026 GMT
  host: www.waikato.ac.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:28:54 2026 GMT
  host: researchcommons.waikato.ac.nz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 21:02:49 2026 GMT
  host: otis.its.waikato.ac.nz
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Waikato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Waikato, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Waikato
provider_slug: university-of-waikato
slug: university-of-waikato-domain-security
source_filename: university-of-waikato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.waikato.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:09:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: researchcommons.waikato.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:28:54 2026 GMT\n  hsts: false\n- host: otis.its.waikato.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:02:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: waikato.ac.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-waikato/refs/heads/main/security/university-of-waikato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Institutional Repository
- Open Access
- New Zealand
---
