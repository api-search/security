---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sliplane.io
  spf: true
hosts:
- cert_expires: Sep 10 22:04:26 2026 GMT
  host: sliplane.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 19:03:29 2026 GMT
  host: docs.sliplane.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 20:07:08 2026 GMT
  host: ctrl.sliplane.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sliplane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sliplane, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sliplane
provider_slug: sliplane
slug: sliplane-domain-security
source_filename: sliplane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sliplane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:04:26 2026 GMT\n  hsts: false\n- host: docs.sliplane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 19:03:29 2026 GMT\n  hsts: false\n- host: ctrl.sliplane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:07:08 2026 GMT\n  hsts: false\ndomains:\n- domain: sliplane.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sliplane/refs/heads/main/security/sliplane-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Container Hosting
- Docker Hosting
- Container As A Service
- Platform As A Service
- Push To Deploy
- Cloud Infrastructure
- European Cloud
- Germany
- Developer Tools
- DevOps
- MCP
---
