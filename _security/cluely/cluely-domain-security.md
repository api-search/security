---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cluely.com
  spf: true
hosts:
- cert_expires: Oct  7 22:40:26 2026 GMT
  host: cluely.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cluely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cluely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cluely
provider_slug: cluely
slug: cluely-domain-security
source_filename: cluely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cluely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 22:40:26 2026 GMT\n  hsts: false\ndomains:\n- domain: cluely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cluely/refs/heads/main/security/cluely-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Meeting Assistant
- Productivity
- Transcription
- Speech Recognition
- Sales
- Real-Time
- Command Line Interface
---
