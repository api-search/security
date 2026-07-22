---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: askdiem.com
  spf: true
hosts:
- cert_expires: Oct 11 03:22:48 2026 GMT
  host: askdiem.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Diem
provider_slug: diem
slug: diem-domain-security
source_filename: diem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askdiem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 03:22:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: askdiem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diem/refs/heads/main/security/diem-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Social
- Search
- Community
- Consumer
- Mobile App
- Women
---
