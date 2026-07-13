---
api_specs:
- filename: luma-labs-openapi.yml
  format: yaml
  label: Luma Dream Machine API
  slug: dream-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-labs/refs/heads/main/openapi/luma-labs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lumalabs.ai
  spf: true
hosts:
- cert_expires: Sep 18 23:09:53 2026 GMT
  host: lumalabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 21:55:43 2026 GMT
  host: docs.lumalabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: api.lumalabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luma Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luma AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Luma AI
provider_slug: luma-labs
slug: luma-labs-domain-security
source_filename: luma-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumalabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:09:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lumalabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:55:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lumalabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lumalabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luma-labs/refs/heads/main/security/luma-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Generative AI
- Video
- Image
- Text To Video
- Image To Video
- Upscaling
- Reframing
- Dream Machine
- Ray
- Photon
- Creative Tools
---
