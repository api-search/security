---
api_specs:
- filename: openapi.json
  format: json
  label: RunPod REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://rest.runpod.io/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: runpod.io
  spf: true
hosts:
- cert_expires: Sep 11 13:26:23 2026 GMT
  host: runpod.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 20:20:23 2026 GMT
  host: console.runpod.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 15:19:59 2026 GMT
  host: docs.runpod.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runpod Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RunPod, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RunPod
provider_slug: runpod
slug: runpod-domain-security
source_filename: runpod-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runpod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:26:23 2026 GMT\n  hsts: false\n- host: console.runpod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:20:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.runpod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:19:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: runpod.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runpod/refs/heads/main/security/runpod-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Cloud
- Compute
- GPU
- Inference
- Machine Learning
- Serverless
---
