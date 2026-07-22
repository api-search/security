---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: transcriptic.com
  spf: true
hosts:
- cert_expires: Sep 21 16:40:41 2026 GMT
  host: transcriptic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transcriptic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transcriptic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transcriptic
provider_slug: transcriptic
slug: transcriptic-domain-security
source_filename: transcriptic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transcriptic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:40:41 2026 GMT\n  hsts: null\ndomains:\n- domain: transcriptic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcriptic/refs/heads/main/security/transcriptic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Laboratory Automation
- Cloud Lab
- Drug Discovery
- Biotechnology
- REST API
- JSON:API
- Autoprotocol
---
