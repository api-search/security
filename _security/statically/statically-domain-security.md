---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: statically.io
  spf: true
hosts:
- cert_expires: Sep 14 20:31:11 2026 GMT
  host: statically.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Statically Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Statically, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Statically
provider_slug: statically
slug: statically-domain-security
source_filename: statically-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: statically.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:31:11 2026 GMT\n  hsts: false\ndomains:\n- domain: statically.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statically/refs/heads/main/security/statically-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Development
- Public APIs
---
