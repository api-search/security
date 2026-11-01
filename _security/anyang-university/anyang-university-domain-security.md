---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: anyang.ac.kr
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: www.anyang.ac.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anyang University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anyang University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Anyang University
provider_slug: anyang-university
slug: anyang-university-domain-security
source_filename: anyang-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anyang.ac.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: anyang.ac.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/anyang-university/security/anyang-university-domain-security.yml
summary_line: TLSv1.3
tags:
- Education
- University
- SouthKorea
- HigherEducation
- Research
---
