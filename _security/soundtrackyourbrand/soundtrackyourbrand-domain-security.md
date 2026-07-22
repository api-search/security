---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soundtrack.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soundtrackyourbrand.com
  spf: true
hosts:
- cert_expires: Sep 18 22:11:09 2026 GMT
  host: www.soundtrack.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 14:59:17 2026 GMT
  host: api.soundtrackyourbrand.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soundtrackyourbrand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soundtrack Your Brand, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Soundtrack Your Brand
provider_slug: soundtrackyourbrand
slug: soundtrackyourbrand-domain-security
source_filename: soundtrackyourbrand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soundtrack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:11:09 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.soundtrackyourbrand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 14:59:17 2026 GMT\n  hsts: null\ndomains:\n- domain: soundtrack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: soundtrackyourbrand.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundtrackyourbrand/refs/heads/main/security/soundtrackyourbrand-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Streaming
- Business Music
- Media
- Entertainment
- GraphQL
- Playback Control
- Retail
---
