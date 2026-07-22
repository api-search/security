---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sinotau.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: sinotau.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sinotau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sinotau, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sinotau
provider_slug: sinotau
slug: sinotau-domain-security
source_filename: sinotau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sinotau.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sinotau.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinotau/refs/heads/main/security/sinotau-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Pharmaceuticals
- Radiopharmaceuticals
- Nuclear Medicine
- Healthcare
- Biotech
- Oncology
- China
---
