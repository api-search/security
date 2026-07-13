---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iitd.ac.in
  spf: true
hosts:
- cert_expires: Sep 20 08:56:01 2026 GMT
  host: home.iitd.ac.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 08:56:01 2026 GMT
  host: ir.iitd.ac.in
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: oauth.iitd.ac.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iit Delhi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Institute of Technology Delhi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Indian Institute of Technology Delhi
provider_slug: iit-delhi
slug: iit-delhi-domain-security
source_filename: iit-delhi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: home.iitd.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ir.iitd.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:56:01 2026 GMT\n  hsts: false\n- host: oauth.iitd.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: iitd.ac.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iit-delhi/refs/heads/main/security/iit-delhi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- India
- Open Access
- Library
---
