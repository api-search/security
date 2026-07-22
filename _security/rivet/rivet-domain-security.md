---
api_specs:
- filename: rivet-rivetkit-openapi.json
  format: json
  label: RivetKit API
  slug: rivetkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivet/refs/heads/main/openapi/rivet-rivetkit-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rivet.dev
  spf: true
hosts:
- cert_expires: Oct  5 21:13:32 2026 GMT
  host: www.rivet.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:16:19 2026 GMT
  host: api.rivet.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rivet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rivet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rivet
provider_slug: rivet
slug: rivet-domain-security
source_filename: rivet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rivet.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:13:32 2026 GMT\n  hsts: false\n- host: api.rivet.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:16:19 2026 GMT\n  hsts: false\ndomains:\n- domain: rivet.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rivet/refs/heads/main/security/rivet-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Infrastructure
- Actors
- Stateful Compute
- AI Agents
- Realtime
- Serverless
- Edge
- WebSockets
- Durable Execution
- Developer Tools
---
