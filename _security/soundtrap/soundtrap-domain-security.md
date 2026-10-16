---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: soundtrap.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: soundtrap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Soundtrap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soundtrap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Soundtrap
provider_slug: soundtrap
slug: soundtrap-domain-security
source_filename: soundtrap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soundtrap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: soundtrap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundtrap/refs/heads/main/security/soundtrap-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Music
- Collaboration
- Education
- Online-DAW
- Soundtrap
---
