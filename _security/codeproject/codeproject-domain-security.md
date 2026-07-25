---
api_specs:
- filename: codeproject-articles-api-openapi.yml
  format: yaml
  label: CodeProject Articles API
  slug: codeproject-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-articles-api-openapi.yml
- filename: codeproject-audio-api-openapi.yml
  format: yaml
  label: CodeProject Audio API
  slug: codeproject-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-audio-api-openapi.yml
- filename: codeproject-forummessages-api-openapi.yml
  format: yaml
  label: CodeProject ForumMessages API
  slug: codeproject-forummessages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-forummessages-api-openapi.yml
- filename: codeproject-image-processing-api-openapi.yml
  format: yaml
  label: CodeProject Image-Processing API
  slug: codeproject-image-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-image-processing-api-openapi.yml
- filename: codeproject-my-api-openapi.yml
  format: yaml
  label: CodeProject My API
  slug: codeproject-my-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-my-api-openapi.yml
- filename: codeproject-questions-api-openapi.yml
  format: yaml
  label: CodeProject Questions API
  slug: codeproject-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-questions-api-openapi.yml
- filename: codeproject-status-api-openapi.yml
  format: yaml
  label: CodeProject Status API
  slug: codeproject-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-status-api-openapi.yml
- filename: codeproject-text-api-openapi.yml
  format: yaml
  label: CodeProject Text API
  slug: codeproject-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-text-api-openapi.yml
- filename: codeproject-training-api-openapi.yml
  format: yaml
  label: CodeProject Training API
  slug: codeproject-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-training-api-openapi.yml
- filename: codeproject-vision-alpr-api-openapi.yml
  format: yaml
  label: CodeProject Vision-ALPR API
  slug: codeproject-vision-alpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-vision-alpr-api-openapi.yml
- filename: codeproject-vision-detection-api-openapi.yml
  format: yaml
  label: CodeProject Vision-Detection API
  slug: codeproject-vision-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-vision-detection-api-openapi.yml
- filename: codeproject-vision-face-api-openapi.yml
  format: yaml
  label: CodeProject Vision-Face API
  slug: codeproject-vision-face-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-vision-face-api-openapi.yml
- filename: codeproject-vision-scene-api-openapi.yml
  format: yaml
  label: CodeProject Vision-Scene API
  slug: codeproject-vision-scene-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-vision-scene-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codeproject.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: codeproject.ai
  spf: false
hosts:
- cert_expires: Oct 21 18:22:05 2026 GMT
  host: www.codeproject.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: codeproject.ai
  https: false
- host: api.codeproject.com
  https: false
kind: domain-security
layout: security
method: probed
name: Codeproject Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeProject, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CodeProject
provider_slug: codeproject
slug: codeproject-domain-security
source_filename: codeproject-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codeproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 18:22:05 2026 GMT\n  hsts: false\n- host: codeproject.ai\n  https: false\n- host: api.codeproject.com\n  https: false\ndomains:\n- domain: codeproject.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: codeproject.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/security/codeproject-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Articles
- Community
- Computer Vision
- Developer Community
- Face Recognition
- Forum
- Knowledge Base
- License Plate Recognition
- Object Detection
- Q&A
- Software Development
- Tutorials
---
