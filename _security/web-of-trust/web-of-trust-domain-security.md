---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mywot.com
  spf: true
hosts:
- cert_expires: Sep 16 23:41:50 2026 GMT
  host: support.mywot.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Web Of Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Web of Trust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Web of Trust
provider_slug: web-of-trust
slug: web-of-trust-domain-security
source_filename: web-of-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: support.mywot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:41:50 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: mywot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web-of-trust/refs/heads/main/security/web-of-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Anti Malware
- Public APIs
---
