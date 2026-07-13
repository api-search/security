---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: voidly.ai
  spf: true
hosts:
- cert_expires: Sep 12 19:30:55 2026 GMT
  host: voidly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voidly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voidly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Voidly
provider_slug: voidly
slug: voidly-domain-security
source_filename: voidly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voidly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:30:55 2026 GMT\n  hsts: false\ndomains:\n- domain: voidly.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voidly/refs/heads/main/security/voidly-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Open Data
- Public APIs
---
