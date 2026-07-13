---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: whereparcel.com
  spf: true
hosts:
- cert_expires: Sep  5 04:38:14 2026 GMT
  host: whereparcel.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whereparcel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WhereParcel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WhereParcel
provider_slug: whereparcel
slug: whereparcel-domain-security
source_filename: whereparcel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whereparcel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:38:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: whereparcel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whereparcel/refs/heads/main/security/whereparcel-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Tracking
- Public APIs
---
