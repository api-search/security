---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wisc.edu
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.wisc.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 02:52:46 2026 GMT
  host: developer.wisc.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 15:17:39 2026 GMT
  host: wams.doit.wisc.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Wisconsin Madison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Wisconsin-Madison, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: University of Wisconsin-Madison
provider_slug: university-of-wisconsin-madison
slug: university-of-wisconsin-madison-domain-security
source_filename: university-of-wisconsin-madison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wisc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\n- host: developer.wisc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:52:46 2026 GMT\n  hsts: null\n- host: wams.doit.wisc.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 15:17:39 2026 GMT\n  hsts: false\ndomains:\n- domain: wisc.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/security/university-of-wisconsin-madison-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Identity
- Student Information System
- Curriculum
- Human Resources
- United States
---
