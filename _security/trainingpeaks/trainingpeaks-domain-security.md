---
api_specs:
- filename: trainingpeaks-athlete-api-openapi.yml
  format: yaml
  label: TrainingPeaks Athlete API
  slug: trainingpeaks-athlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-athlete-api-openapi.yml
- filename: trainingpeaks-coach-api-openapi.yml
  format: yaml
  label: TrainingPeaks Coach API
  slug: trainingpeaks-coach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-coach-api-openapi.yml
- filename: trainingpeaks-events-api-openapi.yml
  format: yaml
  label: TrainingPeaks Events API
  slug: trainingpeaks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-events-api-openapi.yml
- filename: trainingpeaks-file-api-openapi.yml
  format: yaml
  label: TrainingPeaks File API
  slug: trainingpeaks-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-file-api-openapi.yml
- filename: trainingpeaks-info-api-openapi.yml
  format: yaml
  label: TrainingPeaks Info API
  slug: trainingpeaks-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-info-api-openapi.yml
- filename: trainingpeaks-metrics-api-openapi.yml
  format: yaml
  label: TrainingPeaks Metrics API
  slug: trainingpeaks-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-metrics-api-openapi.yml
- filename: trainingpeaks-nutrition-api-openapi.yml
  format: yaml
  label: TrainingPeaks Nutrition API
  slug: trainingpeaks-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-nutrition-api-openapi.yml
- filename: trainingpeaks-routes-api-openapi.yml
  format: yaml
  label: TrainingPeaks Routes API
  slug: trainingpeaks-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-routes-api-openapi.yml
- filename: trainingpeaks-webhooks-api-openapi.yml
  format: yaml
  label: TrainingPeaks Webhooks API
  slug: trainingpeaks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-webhooks-api-openapi.yml
- filename: trainingpeaks-workouts-api-openapi.yml
  format: yaml
  label: TrainingPeaks Workouts API
  slug: trainingpeaks-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-workouts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trainingpeaks.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.trainingpeaks.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.trainingpeaks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.sandbox.trainingpeaks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trainingpeaks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrainingPeaks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TrainingPeaks
provider_slug: trainingpeaks
slug: trainingpeaks-domain-security
source_filename: trainingpeaks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trainingpeaks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.trainingpeaks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\n- host: api.sandbox.trainingpeaks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trainingpeaks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/security/trainingpeaks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Endurance Training
- Workouts
- Coaching
- Sports
- Health
- Wearables
---
