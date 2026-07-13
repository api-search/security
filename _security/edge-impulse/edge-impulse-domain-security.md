---
api_specs:
- filename: edge-impulse-openapi.yml
  format: yaml
  label: Edge Impulse API
  slug: edge-impulse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-impulse/refs/heads/main/openapi/edge-impulse-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: edgeimpulse.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: edgeimpulse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:08:00 2026 GMT
  host: docs.edgeimpulse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: studio.edgeimpulse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edge Impulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edge Impulse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Edge Impulse
provider_slug: edge-impulse
slug: edge-impulse-domain-security
source_filename: edge-impulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edgeimpulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.edgeimpulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:08:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: studio.edgeimpulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: edgeimpulse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edge-impulse/refs/heads/main/security/edge-impulse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Embedded Machine Learning
- Edge AI
---
