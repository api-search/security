---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autocrypt.io
  spf: true
hosts:
- cert_expires: Nov  1 00:01:55 2026 GMT
  host: autocrypt.io
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autocrypt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autocrypt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Autocrypt
provider_slug: autocrypt
slug: autocrypt-domain-security
source_filename: autocrypt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autocrypt.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 00:01:55 2026 GMT\n  hsts: false\ndomains:\n- domain: autocrypt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autocrypt/refs/heads/main/security/autocrypt-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Cybersecurity
- Automotive
- Physical AI
- Mobility
---
