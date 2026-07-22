---
api_specs:
- filename: subspace-openapi-original.yml
  format: yaml
  label: Subspace Product API
  slug: subspace-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subspace/refs/heads/main/openapi/subspace-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: subspace.com
  spf: true
hosts:
- cert_expires: Sep 21 08:09:15 2026 GMT
  host: www.subspace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.subspace.com
  https: false
kind: domain-security
layout: security
method: probed
name: Subspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subspace, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Subspace
provider_slug: subspace
slug: subspace-domain-security
source_filename: subspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.subspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:09:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.subspace.com\n  https: false\ndomains:\n- domain: subspace.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subspace/refs/heads/main/security/subspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Networking
- Real-Time
- WebRTC
- VoIP
- SIP
- CDN
- Gaming
- Latency
- Infrastructure
---
