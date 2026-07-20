---
api_specs:
- filename: landingai-ade-v2-openapi-original.json
  format: json
  label: LandingAI Agentic Document Extraction (ADE) API v2
  slug: ade-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-ade-v2-openapi-original.json
- filename: landingai-ade-v1-openapi-original.json
  format: json
  label: LandingAI Agentic Document Extraction (ADE) API v1
  slug: ade-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-ade-v1-openapi-original.json
- filename: landingai-vision-tools-openapi-original.json
  format: json
  label: LandingAI Vision Tools API
  slug: vision-tools
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-vision-tools-openapi-original.json
- filename: landingai-landinglens-openapi-original.json
  format: json
  label: LandingLens API
  slug: landinglens
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-landinglens-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: landing.ai
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: landing.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:53:29 2026 GMT
  host: docs.landing.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.ade.landing.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landingai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landing.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Landing.ai
provider_slug: landingai
slug: landingai-domain-security
source_filename: landingai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landing.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\n- host: docs.landing.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:53:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ade.landing.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: landing.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/security/landingai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Document Extraction
- Document Processing
- Computer Vision
- OCR
- Data Extraction
- Agents
- Developer Tools
---
