---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biocharnow.com
  spf: false
hosts:
- cert_expires: Nov 11 12:09:47 2026 GMT
  host: biocharnow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biocharnow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biocharnow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Biocharnow
provider_slug: biocharnow
slug: biocharnow-domain-security
source_filename: biocharnow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biocharnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 12:09:47 2026 GMT\n  hsts: false\ndomains:\n- domain: biocharnow.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biocharnow/refs/heads/main/security/biocharnow-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biochar
- Sustainability
- Agriculture
- Manufacturing
---
