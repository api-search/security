---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: curl.se
  spf: true
hosts:
- cert_expires: Sep  3 15:38:23 2026 GMT
  host: curl.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cURL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: cURL
provider_slug: curl
slug: curl-domain-security
source_filename: curl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curl.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 15:38:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curl.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curl/refs/heads/main/security/curl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Client
- Command Line
- Data Transfer
- FTP
- HTTP
- HTTPS
- Library
- Network Tools
- Open Source
- REST
---
