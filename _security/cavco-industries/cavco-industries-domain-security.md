---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cavco.com
  spf: true
hosts:
- cert_expires: Oct  6 02:09:06 2026 GMT
  host: www.cavco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.cavco.com
  https: false
- host: api.cavco.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cavco Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cavco Industries, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cavco Industries
provider_slug: cavco-industries
slug: cavco-industries-domain-security
source_filename: cavco-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cavco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:09:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.cavco.com\n  https: false\n- host: api.cavco.com\n  https: false\ndomains:\n- domain: cavco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cavco-industries/refs/heads/main/security/cavco-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufactured Homes
- Housing
---
