---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: studentaid.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ed.gov
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: studentaid.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 23:59:59 2026 GMT
  host: collegescorecard.ed.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 14:20:54 2026 GMT
  host: api.data.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federal Student Aid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Student Aid, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Student Aid
provider_slug: federal-student-aid
slug: federal-student-aid-domain-security
source_filename: federal-student-aid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: studentaid.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: collegescorecard.ed.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:20:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: studentaid.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ed.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-student-aid/refs/heads/main/security/federal-student-aid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Federal Government
- Financial Aid
- Grants
- Loans
- Student Aid
---
