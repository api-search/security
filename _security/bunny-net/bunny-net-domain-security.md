---
api_specs:
- filename: bunny-net-openapi.yml
  format: yaml
  label: Bunny.net Core Platform API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/openapi/bunny-net-openapi.yml
- filename: bunny-net-stream-webhooks-asyncapi.yml
  format: yaml
  label: Bunny.net Stream Webhooks
  slug: stream-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/asyncapi/bunny-net-stream-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bunny.net
  spf: true
hosts:
- cert_expires: Oct  2 02:02:04 2026 GMT
  host: bunny.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 18:12:10 2026 GMT
  host: docs.bunny.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:02:16 2026 GMT
  host: api.bunny.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bunny Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bunny.net, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bunny.net
provider_slug: bunny-net
slug: bunny-net-domain-security
source_filename: bunny-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bunny.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:02:04 2026 GMT\n  hsts: false\n- host: docs.bunny.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:12:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bunny.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:02:16 2026 GMT\n  hsts: false\ndomains:\n- domain: bunny.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunny-net/refs/heads/main/security/bunny-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CDN
- Edge
- Video
- Storage
- DNS
- WAF
- Edge Compute
- Image Optimization
---
