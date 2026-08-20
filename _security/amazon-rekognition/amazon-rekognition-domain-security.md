---
api_specs:
- filename: amazon-rekognition-celebrity-recognition-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Celebrity Recognition API
  slug: amazon-rekognition-celebrity-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-celebrity-recognition-api-openapi.yml
- filename: amazon-rekognition-content-moderation-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Content Moderation API
  slug: amazon-rekognition-content-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-content-moderation-api-openapi.yml
- filename: amazon-rekognition-custom-labels-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Custom Labels API
  slug: amazon-rekognition-custom-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-custom-labels-api-openapi.yml
- filename: amazon-rekognition-face-collections-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Collections API
  slug: amazon-rekognition-face-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-collections-api-openapi.yml
- filename: amazon-rekognition-face-liveness-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Liveness API
  slug: amazon-rekognition-face-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-liveness-api-openapi.yml
- filename: amazon-rekognition-face-search-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Search API
  slug: amazon-rekognition-face-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-search-api-openapi.yml
- filename: amazon-rekognition-facial-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Facial Analysis API
  slug: amazon-rekognition-facial-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-facial-analysis-api-openapi.yml
- filename: amazon-rekognition-image-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Image Analysis API
  slug: amazon-rekognition-image-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-image-analysis-api-openapi.yml
- filename: amazon-rekognition-stored-video-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Stored Video Analysis API
  slug: amazon-rekognition-stored-video-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-stored-video-analysis-api-openapi.yml
- filename: amazon-rekognition-text-detection-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Text Detection API
  slug: amazon-rekognition-text-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-text-detection-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: rekognition.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Rekognition Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Rekognition, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
slug: amazon-rekognition-domain-security
source_filename: amazon-rekognition-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: rekognition.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/security/amazon-rekognition-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Celebrity Recognition
- Computer-Vision
- Content Moderation
- Custom Labels
- Deep Learning
- Face Liveness
- Facial Recognition
- Image Analysis
- Machine-Learning
- Object Detection
- Text Detection
- Video Analysis
---
