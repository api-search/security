---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: texaco.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.texaco.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Texaco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Texaco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Texaco
provider_slug: texaco
slug: texaco-domain-security
source_filename: texaco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.texaco.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: texaco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texaco/refs/heads/main/security/texaco-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Energy
- Oil & Gas
- Retail
---
