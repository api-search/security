---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: drawio.com
  spf: false
hosts:
- cert_expires: Dec 20 08:14:16 2026 GMT
  host: drawio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Drawio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for draw.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: draw.io
provider_slug: drawio
slug: drawio-domain-security
source_filename: drawio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drawio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 08:14:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: drawio.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/drawio/security/drawio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Diagramming
- Collaboration
- OpenSource
- Privacy
- Integration
- Cloud
---
