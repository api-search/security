---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audiodraft.com
  spf: true
hosts:
- cert_expires: Mar 24 13:13:02 2027 GMT
  host: audiodraft.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Audiodraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audiodraft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Audiodraft
provider_slug: audiodraft
slug: audiodraft-domain-security
source_filename: audiodraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiodraft.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 13:13:02 2027 GMT\n  hsts: false\ndomains:\n- domain: audiodraft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audiodraft/refs/heads/main/security/audiodraft-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Audio Branding
- Sound Design
- Music Production
- Voice-over
- Crowdsourcing
- Creative Services
- Audio
---
