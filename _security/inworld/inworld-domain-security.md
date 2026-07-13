---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inworld.ai
  spf: true
hosts:
- cert_expires: Aug 15 17:52:28 2026 GMT
  host: inworld.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 05:53:44 2026 GMT
  host: docs.inworld.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:31:09 2026 GMT
  host: api.inworld.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inworld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inworld AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Inworld AI
provider_slug: inworld
slug: inworld-domain-security
source_filename: inworld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inworld.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 17:52:28 2026 GMT\n  hsts: false\n- host: docs.inworld.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:53:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.inworld.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:31:09 2026 GMT\n  hsts: false\ndomains:\n- domain: inworld.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inworld/refs/heads/main/security/inworld-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Voice
- Characters
- Games
- Conversational
---
