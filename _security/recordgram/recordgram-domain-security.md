---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cre8tor.app
  spf: false
hosts:
- cert_expires: Sep  8 00:20:18 2026 GMT
  host: cre8tor.app
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Recordgram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recordgram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Recordgram
provider_slug: recordgram
slug: recordgram-domain-security
source_filename: recordgram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cre8tor.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 00:20:18 2026 GMT\n  hsts: false\ndomains:\n- domain: cre8tor.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recordgram/refs/heads/main/security/recordgram-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Music
- Music Creation
- Audio
- Recording
- Media and Entertainment
- Consumer App
- Mobile
---
