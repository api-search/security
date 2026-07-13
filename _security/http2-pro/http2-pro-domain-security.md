---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: http2.pro
  spf: false
hosts:
- cert_expires: Aug 31 10:27:48 2026 GMT
  host: http2.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Http2 Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTTP2.Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HTTP2.Pro
provider_slug: http2-pro
slug: http2-pro-domain-security
source_filename: http2-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: http2.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:27:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: http2.pro\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/http2-pro/refs/heads/main/security/http2-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Development
- Public APIs
---
