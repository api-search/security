---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myaccesshope.org
  spf: true
hosts:
- cert_expires: Oct  8 07:42:30 2026 GMT
  host: www.myaccesshope.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: app.myaccesshope.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: member/staff portal, credentialed; robots.txt Disallow /
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: docs.myaccesshope.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: document portal behind login; not developer documentation
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accesshope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AccessHope, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AccessHope
provider_slug: accesshope
slug: accesshope-domain-security
source_filename: accesshope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myaccesshope.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:42:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.myaccesshope.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: member/staff portal, credentialed; robots.txt Disallow /\n- host: docs.myaccesshope.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: document portal behind login; not developer documentation\ndomains:\n- domain: myaccesshope.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accesshope/refs/heads/main/security/accesshope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Oncology
- Cancer Care
- Employee Benefits
- Health Benefits
- Digital Health
- Telehealth
- Second Opinion
- Employer Health
---
