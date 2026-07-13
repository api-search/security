---
api_specs:
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Samples API
  slug: samples
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Labels API
  slug: labels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Labelsets API
  slug: labelsets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
- filename: segments-ai-openapi.yml
  format: yaml
  label: Segments.ai Releases API
  slug: releases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/openapi/segments-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: segments.ai
  spf: true
hosts:
- cert_expires: Sep 14 23:37:43 2026 GMT
  host: segments.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:33:26 2026 GMT
  host: docs.segments.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 03:55:56 2026 GMT
  host: api.segments.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Segments Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Segments.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Segments.ai
provider_slug: segments-ai
slug: segments-ai-domain-security
source_filename: segments-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: segments.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:37:43 2026 GMT\n  hsts: false\n- host: docs.segments.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:33:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.segments.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 03:55:56 2026 GMT\n  hsts: null\ndomains:\n- domain: segments.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segments-ai/refs/heads/main/security/segments-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Labeling
- Computer Vision
- Point Cloud
- Annotation
- Machine Learning
---
