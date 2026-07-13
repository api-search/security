---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blague.xyz
  spf: false
hosts:
- cert_expires: Sep 11 04:56:27 2026 GMT
  host: blague.xyz
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Blague Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blague.xyz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Blague.xyz
provider_slug: blague-xyz
slug: blague-xyz-domain-security
source_filename: blague-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blague.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 04:56:27 2026 GMT\n  hsts: null\ndomains:\n- domain: blague.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blague-xyz/refs/heads/main/security/blague-xyz-domain-security.yml
summary_line: TLSv1.2
tags:
- Development
- Public APIs
---
