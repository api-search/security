---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qidz.com
  spf: true
hosts:
- cert_expires: Sep 25 09:01:49 2026 GMT
  host: qidz.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Qidz Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QiDZ Holding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: QiDZ Holding
provider_slug: qidz-holding
slug: qidz-holding-domain-security
source_filename: qidz-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qidz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 09:01:49 2026 GMT\n  hsts: null\ndomains:\n- domain: qidz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qidz-holding/refs/heads/main/security/qidz-holding-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Family Activities
- Events
- Booking
- Entertainment
- Mobile App
- Consumer
- UAE
- Middle East
- Discovery
---
