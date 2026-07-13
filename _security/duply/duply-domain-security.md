---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: duply.co
  spf: true
hosts:
- cert_expires: Aug  9 20:08:07 2026 GMT
  host: duply.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Duply
provider_slug: duply
slug: duply-domain-security
source_filename: duply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duply.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 20:08:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: duply.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duply/refs/heads/main/security/duply-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Photography
- Public APIs
---
