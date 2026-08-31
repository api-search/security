---
api_specs:
- filename: leia-media-transformation-api-openapi.yml
  format: yaml
  label: Leia Media Transformation API
  slug: leia-media-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-media-transformation-api-openapi.yml
- filename: leia-product-pricing-api-openapi.yml
  format: yaml
  label: Leia Product Pricing API
  slug: leia-product-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-product-pricing-api-openapi.yml
- filename: leia-protocol-api-openapi.yml
  format: yaml
  label: Leia Protocol API
  slug: leia-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-protocol-api-openapi.yml
- filename: leia-storage-api-openapi.yml
  format: yaml
  label: Leia Storage API
  slug: leia-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-storage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: immersity.ai
  spf: true
hosts:
- cert_expires: Oct 15 08:19:16 2026 GMT
  host: immersity.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 07:01:51 2026 GMT
  host: docs-api.immersity.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: api.immersity.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Leia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Leia
provider_slug: leia
slug: leia-domain-security
source_filename: leia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immersity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 08:19:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs-api.immersity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.immersity.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: immersity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/security/leia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3D
- Spatial Computing
- Computer-Vision
- depth-estimation
- Image Processing
- Video Processing
- Generative AI
- Displays
- media-transformation
- Immersive Experiences
---
