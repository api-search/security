---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sydney.edu.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usyd.edu.au
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: www.sydney.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:28:22 2026 GMT
  host: ses.library.usyd.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: sydney.primo.exlibrisgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Sydney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Sydney, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Sydney
provider_slug: university-of-sydney
slug: university-of-sydney-domain-security
source_filename: university-of-sydney-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sydney.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\n- host: ses.library.usyd.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:28:22 2026 GMT\n  hsts: false\n- host: sydney.primo.exlibrisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sydney.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: usyd.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sydney/refs/heads/main/security/university-of-sydney-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Library
- Research
- Open Data
- Australia
---
