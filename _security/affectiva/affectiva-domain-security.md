---
api_specs:
- filename: affectiva-annotations-api-openapi.yml
  format: yaml
  label: Affectiva Annotations API
  slug: affectiva-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-annotations-api-openapi.yml
- filename: affectiva-data-collection-projects-api-openapi.yml
  format: yaml
  label: Affectiva data collection projects API
  slug: affectiva-data-collection-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-data-collection-projects-api-openapi.yml
- filename: affectiva-entries-api-openapi.yml
  format: yaml
  label: Affectiva Entries API
  slug: affectiva-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-entries-api-openapi.yml
- filename: affectiva-event-configs-api-openapi.yml
  format: yaml
  label: Affectiva event configs API
  slug: affectiva-event-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-event-configs-api-openapi.yml
- filename: affectiva-event-instances-api-openapi.yml
  format: yaml
  label: Affectiva event instances API
  slug: affectiva-event-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-event-instances-api-openapi.yml
- filename: affectiva-frame-sampling-jobs-api-openapi.yml
  format: yaml
  label: Affectiva frame sampling jobs API
  slug: affectiva-frame-sampling-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-frame-sampling-jobs-api-openapi.yml
- filename: affectiva-jobs-api-openapi.yml
  format: yaml
  label: Affectiva Jobs API
  slug: affectiva-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-jobs-api-openapi.yml
- filename: affectiva-labeling-job-annotations-api-openapi.yml
  format: yaml
  label: Affectiva Labeling Job Annotations API
  slug: affectiva-labeling-job-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-labeling-job-annotations-api-openapi.yml
- filename: affectiva-labeling-jobs-api-openapi.yml
  format: yaml
  label: Affectiva Labeling Jobs API
  slug: affectiva-labeling-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-labeling-jobs-api-openapi.yml
- filename: affectiva-labeling-tasks-api-openapi.yml
  format: yaml
  label: Affectiva Labeling Tasks API
  slug: affectiva-labeling-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-labeling-tasks-api-openapi.yml
- filename: affectiva-representation-storages-api-openapi.yml
  format: yaml
  label: Affectiva representation storages API
  slug: affectiva-representation-storages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-representation-storages-api-openapi.yml
- filename: affectiva-representations-api-openapi.yml
  format: yaml
  label: Affectiva Representations API
  slug: affectiva-representations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-representations-api-openapi.yml
- filename: affectiva-video-frames-api-openapi.yml
  format: yaml
  label: Affectiva Video Frames API
  slug: affectiva-video-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-video-frames-api-openapi.yml
- filename: affectiva-video-segments-api-openapi.yml
  format: yaml
  label: Affectiva Video Segments API
  slug: affectiva-video-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-video-segments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: affectiva.com
  spf: true
hosts:
- cert_expires: Nov  6 22:26:18 2026 GMT
  host: www.affectiva.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: index.affectiva.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Affectiva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affectiva, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Affectiva
provider_slug: affectiva
slug: affectiva-domain-security
source_filename: affectiva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.affectiva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 22:26:18 2026 GMT\n  hsts: false\n- host: index.affectiva.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: affectiva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/security/affectiva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Emotion AI
- Artificial Intelligence
- Machine-Learning
- Computer-Vision
- Facial Coding
- Facial Expression Analysis
- Media Analytics
- Market Research
- Automotive
- Driver Monitoring
- Video Analysis
- Affective Computing
---
