---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jsonbin.io
  spf: true
hosts:
- cert_expires: Oct  5 01:44:08 2026 GMT
  host: jsonbin.io
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jsonbin Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JSONbin.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JSONbin.io
provider_slug: jsonbin-io
slug: jsonbin-io-domain-security
source_filename: jsonbin-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jsonbin.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 01:44:08 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: jsonbin.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jsonbin-io/refs/heads/main/security/jsonbin-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development
- Public APIs
---
