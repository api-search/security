---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tau.ac.il
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exlibrisgroup.com
  spf: true
hosts:
- cert_expires: Jan  1 13:08:08 2027 GMT
  host: english.tau.ac.il
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: tau.primo.exlibrisgroup.com
  hsts: true
  hsts_max_age: 1209600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: developers.exlibrisgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tel Aviv University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tel Aviv University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tel Aviv University
provider_slug: tel-aviv-university
slug: tel-aviv-university-domain-security
source_filename: tel-aviv-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: english.tau.ac.il\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 13:08:08 2027 GMT\n  hsts: false\n- host: tau.primo.exlibrisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 1209600\n- host: developers.exlibrisgroup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tau.ac.il\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: exlibrisgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tel-aviv-university/refs/heads/main/security/tel-aviv-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Israel
- Library
- Discovery
- Research
---
