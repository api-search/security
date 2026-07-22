---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kaiseraluminum.com
  spf: true
hosts:
- cert_expires: Aug 15 19:31:24 2026 GMT
  host: www.kaiseraluminum.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaiser Aluminum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaiser Aluminum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kaiser Aluminum
provider_slug: kaiser-aluminum
slug: kaiser-aluminum-domain-security
source_filename: kaiser-aluminum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kaiseraluminum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 19:31:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kaiseraluminum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaiser-aluminum/refs/heads/main/security/kaiser-aluminum-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Manufacturing
- Aluminum
- Aerospace
- Packaging
- Automotive
---
