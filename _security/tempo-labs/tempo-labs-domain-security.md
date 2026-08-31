---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tempo.new
  spf: true
hosts:
- cert_expires: Sep 24 19:38:53 2026 GMT
  host: tempo.new
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 17:53:21 2026 GMT
  host: docs.tempo.new
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tempo Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tempo Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tempo Labs
provider_slug: tempo-labs
slug: tempo-labs-domain-security
source_filename: tempo-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tempo.new\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:38:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tempo.new\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:53:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tempo.new\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tempo-labs/refs/heads/main/security/tempo-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI App Builder
- Design to Code
- Prompt to Code
- Low Code
- React
- Next.js
- Developer Tools
---
