---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mogassam.com
  spf: true
hosts:
- cert_expires: Dec 14 13:29:09 2026 GMT
  host: mogassam.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mogassam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mogassam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mogassam
provider_slug: mogassam
slug: mogassam-domain-security
source_filename: mogassam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mogassam.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 14 13:29:09 2026 GMT\n  hsts: false\ndomains:\n- domain: mogassam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mogassam/refs/heads/main/security/mogassam-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Dental
- 3D Printing
- Digital Dentistry
- Healthcare
- Manufacturing
- Hardware
---
