---
api_specs:
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Athlete API
  slug: trainingpeaks-athlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workouts API
  slug: trainingpeaks-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workout Details API
  slug: trainingpeaks-workout-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Workout of the Day API
  slug: trainingpeaks-workout-of-the-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Metrics API
  slug: trainingpeaks-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Nutrition API
  slug: trainingpeaks-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Coach API
  slug: trainingpeaks-coach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks File Upload API
  slug: trainingpeaks-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Events and Routes API
  slug: trainingpeaks-events-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
- filename: trainingpeaks-openapi.yml
  format: yaml
  label: TrainingPeaks Webhooks API
  slug: trainingpeaks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/openapi/trainingpeaks-openapi.yml
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
