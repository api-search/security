---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freetts.org
  spf: true
hosts:
- cert_expires: Oct 21 05:10:07 2026 GMT
  host: freetts.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freetts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeTTS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FreeTTS
provider_slug: freetts
slug: freetts-domain-security
source_filename: freetts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freetts.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 05:10:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: freetts.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freetts/refs/heads/main/security/freetts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Text-to-Speech
- Speech Synthesis
- AI Voice
- Audio
- Media
- Accessibility
- Speech-to-Text
- Content Creation
- Developer Tools
---
