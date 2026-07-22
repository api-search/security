---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: m.io
  spf: true
hosts:
- cert_expires: Oct  8 08:33:53 2026 GMT
  host: www.m.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mio
provider_slug: mio
slug: mio-domain-security
source_filename: mio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.m.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: m.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mio/refs/heads/main/security/mio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Collaboration
- Interoperability
- Messaging
- Enterprise
- Directory Sync
- Google Workspace
- Microsoft 365
- Slack
- Zoom
---
