---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "emsign.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: case.edu
  spf: true
hosts:
- cert_expires: Sep  6 13:59:05 2026 GMT
  host: case.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: login.case.edu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 15 12:15:22 2026 GMT
  host: researchguides.case.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Case Western Reserve University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Case Western Reserve University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Case Western Reserve University
provider_slug: case-western-reserve-university
slug: case-western-reserve-university-domain-security
source_filename: case-western-reserve-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: case.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:59:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: login.case.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: researchguides.case.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 12:15:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: case.edu\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"emsign.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/case-western-reserve-university/refs/heads/main/security/case-western-reserve-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Cleveland
- Ohio
- United States
---
