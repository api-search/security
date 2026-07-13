---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: veriphone.io
  spf: true
hosts:
- cert_expires: Aug 20 04:38:17 2026 GMT
  host: veriphone.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veriphone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veriphone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Veriphone
provider_slug: veriphone
slug: veriphone-domain-security
source_filename: veriphone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veriphone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:38:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: veriphone.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veriphone/refs/heads/main/security/veriphone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Phone
- Public APIs
---
