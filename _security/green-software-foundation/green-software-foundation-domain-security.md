---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greensoftware.foundation
  spf: false
hosts:
- cert_expires: Aug 18 01:27:58 2026 GMT
  host: greensoftware.foundation
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Software Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Software Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Green Software Foundation
provider_slug: green-software-foundation
slug: green-software-foundation-domain-security
source_filename: green-software-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greensoftware.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:27:58 2026 GMT\n  hsts: false\ndomains:\n- domain: greensoftware.foundation\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-software-foundation/refs/heads/main/security/green-software-foundation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Carbon
- Linux Foundation
- Software
- Sustainability
---
