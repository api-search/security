---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: major.io
  spf: true
hosts:
- cert_expires: Sep  8 02:53:51 2026 GMT
  host: major.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Icanhazip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Icanhazip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Icanhazip
provider_slug: icanhazip
slug: icanhazip-domain-security
source_filename: icanhazip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: major.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 02:53:51 2026 GMT\n  hsts: false\ndomains:\n- domain: major.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icanhazip/refs/heads/main/security/icanhazip-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---
