---
api_specs:
- filename: landingai-classes-api-openapi.yml
  format: yaml
  label: Landing.ai Classes API
  slug: landingai-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-classes-api-openapi.yml
- filename: landingai-deployment-api-openapi.yml
  format: yaml
  label: Landing.ai Deployment API
  slug: landingai-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-deployment-api-openapi.yml
- filename: landingai-extract-api-openapi.yml
  format: yaml
  label: Landing.ai Extract API
  slug: landingai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-extract-api-openapi.yml
- filename: landingai-image-api-openapi.yml
  format: yaml
  label: Landing.ai Image API
  slug: landingai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-image-api-openapi.yml
- filename: landingai-metadata-api-openapi.yml
  format: yaml
  label: Landing.ai Metadata API
  slug: landingai-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-metadata-api-openapi.yml
- filename: landingai-metrics-api-openapi.yml
  format: yaml
  label: Landing.ai Metrics API
  slug: landingai-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-metrics-api-openapi.yml
- filename: landingai-model-api-openapi.yml
  format: yaml
  label: Landing.ai Model API
  slug: landingai-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-model-api-openapi.yml
- filename: landingai-parse-api-openapi.yml
  format: yaml
  label: Landing.ai Parse API
  slug: landingai-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-parse-api-openapi.yml
- filename: landingai-project-api-openapi.yml
  format: yaml
  label: Landing.ai Project API
  slug: landingai-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-project-api-openapi.yml
- filename: landingai-snapshot-api-openapi.yml
  format: yaml
  label: Landing.ai Snapshot API
  slug: landingai-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-snapshot-api-openapi.yml
- filename: landingai-tags-api-openapi.yml
  format: yaml
  label: Landing.ai Tags API
  slug: landingai-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-tags-api-openapi.yml
- filename: landingai-tools-api-openapi.yml
  format: yaml
  label: Landing.ai Tools API
  slug: landingai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-tools-api-openapi.yml
- filename: landingai-training-api-openapi.yml
  format: yaml
  label: Landing.ai Training API
  slug: landingai-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-training-api-openapi.yml
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
- Machine-Learning
- Document Extraction
- Document Processing
- Computer-Vision
- OCR
- Data Extraction
- Agents
- Developer Tools
---
