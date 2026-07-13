---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cleanuri.com
  spf: false
hosts:
- cert_expires: Aug 13 23:07:58 2026 GMT
  host: cleanuri.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cleanuri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CleanURI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CleanURI
provider_slug: cleanuri
slug: cleanuri-domain-security
source_filename: cleanuri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cleanuri.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 13 23:07:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cleanuri.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanuri/refs/heads/main/security/cleanuri-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- URL Shorteners
- Public APIs
---
