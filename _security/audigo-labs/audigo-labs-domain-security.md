---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audigolabs.com
  spf: true
hosts:
- cert_expires: Sep  3 06:48:02 2026 GMT
  host: audigolabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Audigo Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audigo Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Audigo Labs
provider_slug: audigo-labs
slug: audigo-labs-domain-security
source_filename: audigo-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audigolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 06:48:02 2026 GMT\n  hsts: null\ndomains:\n- domain: audigolabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audigo-labs/refs/heads/main/security/audigo-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Audio
- Music
- Recording
- Consumer Hardware
- Mobile App
- Microphones
- Content Creation
- Agentic Commerce
---
