---
api_specs:
- filename: vital-users-api-openapi.yml
  format: yaml
  label: Vital Users API
  slug: vital-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-users-api-openapi.yml
- filename: vital-link-api-openapi.yml
  format: yaml
  label: Vital Link API
  slug: vital-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-link-api-openapi.yml
- filename: vital-wearables-api-openapi.yml
  format: yaml
  label: Vital Wearables Data API
  slug: vital-wearables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-wearables-api-openapi.yml
- filename: vital-lab-testing-api-openapi.yml
  format: yaml
  label: Vital Lab Testing API
  slug: vital-lab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-lab-testing-api-openapi.yml
- filename: vital-lab-report-parser-api-openapi.yml
  format: yaml
  label: Vital Lab Report Parser API
  slug: vital-lab-report-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-lab-report-parser-api-openapi.yml
- filename: vital-sense-api-openapi.yml
  format: yaml
  label: Vital Sense API
  slug: vital-sense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-sense-api-openapi.yml
- filename: vital-team-api-openapi.yml
  format: yaml
  label: Vital Team API
  slug: vital-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-team-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: junction.com
  spf: true
hosts:
- cert_expires: Sep 25 05:23:47 2026 GMT
  host: www.junction.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 12:00:15 2026 GMT
  host: docs.junction.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 11:38:31 2026 GMT
  host: api.us.junction.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vital Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vital, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vital
provider_slug: vital-io
slug: vital-io-domain-security
source_filename: vital-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.junction.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.junction.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:00:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.us.junction.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 11:38:31 2026 GMT\n  hsts: null\ndomains:\n- domain: junction.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/security/vital-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health Data
- Wearables
- Lab Testing
- Digital Health
- Healthtech
- Healthcare
- HIPAA
- HealthKit
- Health Connect
- EHR
- EMR
- Biomarkers
- Diagnostics
- Continuous Glucose Monitoring
- Sleep
- Activity
- Heart Rate
- Webhooks
- Phlebotomy
- Lab Orders
---
