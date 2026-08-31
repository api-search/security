---
api_specs:
- filename: krea-ai-assets-api-openapi.yml
  format: yaml
  label: Krea Assets API
  slug: krea-ai-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-assets-api-openapi.yml
- filename: krea-ai-general-api-openapi.yml
  format: yaml
  label: Krea General API
  slug: krea-ai-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-general-api-openapi.yml
- filename: krea-ai-image-api-openapi.yml
  format: yaml
  label: Krea Image API
  slug: krea-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-image-api-openapi.yml
- filename: krea-ai-image-enhance-api-openapi.yml
  format: yaml
  label: Krea Image Enhance API
  slug: krea-ai-image-enhance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-image-enhance-api-openapi.yml
- filename: krea-ai-node-apps-api-openapi.yml
  format: yaml
  label: Krea Node Apps API
  slug: krea-ai-node-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-node-apps-api-openapi.yml
- filename: krea-ai-styles-api-openapi.yml
  format: yaml
  label: Krea Styles API
  slug: krea-ai-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-styles-api-openapi.yml
- filename: krea-ai-video-api-openapi.yml
  format: yaml
  label: Krea Video API
  slug: krea-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/openapi/krea-ai-video-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: krea.ai
  spf: true
hosts:
- cert_expires: Aug 28 11:16:20 2026 GMT
  host: www.krea.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 05:02:27 2026 GMT
  host: docs.krea.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 19:01:03 2026 GMT
  host: api.krea.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Krea Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Krea, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Krea
provider_slug: krea-ai
slug: krea-ai-domain-security
source_filename: krea-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.krea.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:16:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.krea.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.krea.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:01:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: krea.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/krea-ai/refs/heads/main/security/krea-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Image-Generation
- Video Generation
- Generative AI
- Real-Time
- Multimodal
- Creative Tools
- 3D
- Upscaling
---
