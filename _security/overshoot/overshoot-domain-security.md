---
api_specs:
- filename: overshoot-openapi.yaml
  format: yaml
  label: Overshoot API
  slug: overshoot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: overshoot.ai
  spf: true
hosts:
- cert_expires: Sep 27 16:16:51 2026 GMT
  host: docs.overshoot.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:47:31 2026 GMT
  host: api.overshoot.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overshoot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overshoot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Overshoot
provider_slug: overshoot
slug: overshoot-domain-security
source_filename: overshoot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.overshoot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:16:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.overshoot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:47:31 2026 GMT\n  hsts: null\ndomains:\n- domain: overshoot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/security/overshoot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Video
- Video Understanding
- Vision Language Models
- Real Time
- Streaming
- WebRTC
- Inference
- Multimodal
- Machine Learning
---
