---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: princetonreview.com
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.princetonreview.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Education Holdings 1 The Princeton Review Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Education Holdings 1 (The Princeton Review), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Education Holdings 1 (The Princeton Review)
provider_slug: education-holdings-1-the-princeton-review
slug: education-holdings-1-the-princeton-review-domain-security
source_filename: education-holdings-1-the-princeton-review-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.princetonreview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: princetonreview.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/education-holdings-1-the-princeton-review/refs/heads/main/security/education-holdings-1-the-princeton-review-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- Education
- Test Prep
- Tutoring
- Admissions
- EdTech
- Consumer
---
