---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: at-home-doc.com
  spf: true
hosts:
- cert_expires: Oct 12 09:43:32 2026 GMT
  host: at-home-doc.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: At Home Doc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for At-Home-Doc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: At-Home-Doc
provider_slug: at-home-doc
slug: at-home-doc-domain-security
source_filename: at-home-doc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: at-home-doc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 09:43:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: at-home-doc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-home-doc/refs/heads/main/security/at-home-doc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Telemedicine
- Telehealth
- Digital Health
- Home Care
- Pharmacy
- Qatar
- Mobile App
---
