---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mosanna.com
  spf: true
hosts:
- cert_expires: Sep  9 15:03:09 2026 GMT
  host: mosanna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mosanna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mosanna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mosanna
provider_slug: mosanna
slug: mosanna-domain-security
source_filename: mosanna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mosanna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 15:03:09 2026 GMT\n  hsts: false\ndomains:\n- domain: mosanna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosanna/refs/heads/main/security/mosanna-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Healthcare
- Sleep Apnea
- Therapeutics
---
