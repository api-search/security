---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: canvasgfx.com
  spf: true
hosts:
- cert_expires: Dec 14 08:02:30 2026 GMT
  host: canvasgfx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canvasgfx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canvasgfx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Canvasgfx
provider_slug: canvasgfx
slug: canvasgfx-domain-security
source_filename: canvasgfx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canvasgfx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 08:02:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: canvasgfx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvasgfx/refs/heads/main/security/canvasgfx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- AI
- Knowledge-Management
- Cloud
---
