---
api_specs:
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Personal Info API
  slug: oura-personal-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Daily Summaries API
  slug: oura-daily-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Sleep API
  slug: oura-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Activity API
  slug: oura-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Heart Rate API
  slug: oura-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Tags API
  slug: oura-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Ring Configuration API
  slug: oura-ring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Webhooks API
  slug: oura-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
- filename: oura-api-openapi.yml
  format: yaml
  label: Oura Sandbox API
  slug: oura-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/openapi/oura-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@ouraring.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ouraring.com
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: ouraring.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: cloud.ouraring.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oura Ring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oura, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oura
provider_slug: oura-ring
slug: oura-ring-domain-security
source_filename: oura-ring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ouraring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.ouraring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ouraring.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@ouraring.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oura-ring/refs/heads/main/security/oura-ring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Activity
- Biometrics
- Cardiovascular
- Fitness
- Health
- HRV
- Quantified Self
- Readiness
- Resilience
- Ring
- Sleep
- SpO2
- Stress
- Wearables
- Wellness
- Women's Health
---
