---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: the-one-api.dev
  spf: false
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: the-one-api.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Lord Of The Rings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Lord of the Rings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: The Lord of the Rings
provider_slug: the-lord-of-the-rings
slug: the-lord-of-the-rings-domain-security
source_filename: the-lord-of-the-rings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: the-one-api.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: the-one-api.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-lord-of-the-rings/refs/heads/main/security/the-lord-of-the-rings-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Video
- Public APIs
---
