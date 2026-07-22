---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nstream.io
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.nstream.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nstream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nstream
provider_slug: nstream
slug: nstream-domain-security
source_filename: nstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nstream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nstream.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nstream/refs/heads/main/security/nstream-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Streaming
- Real-Time
- Event Streaming
- Stateful Services
- Streaming APIs
- Data Connectors
- Open Source
- WebSockets
- SwimOS
---
