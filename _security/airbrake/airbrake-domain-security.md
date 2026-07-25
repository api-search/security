---
api_specs:
- filename: airbrake-activities-api-openapi.yml
  format: yaml
  label: Airbrake Activities API
  slug: airbrake-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-activities-api-openapi.yml
- filename: airbrake-deploys-api-openapi.yml
  format: yaml
  label: Airbrake Deploys API
  slug: airbrake-deploys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-deploys-api-openapi.yml
- filename: airbrake-groups-api-openapi.yml
  format: yaml
  label: Airbrake Groups API
  slug: airbrake-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-groups-api-openapi.yml
- filename: airbrake-ios-crash-reports-api-openapi.yml
  format: yaml
  label: Airbrake iOS Crash Reports API
  slug: airbrake-ios-crash-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-ios-crash-reports-api-openapi.yml
- filename: airbrake-notices-api-openapi.yml
  format: yaml
  label: Airbrake Notices API
  slug: airbrake-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-notices-api-openapi.yml
- filename: airbrake-performance-api-openapi.yml
  format: yaml
  label: Airbrake Performance API
  slug: airbrake-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-performance-api-openapi.yml
- filename: airbrake-projects-api-openapi.yml
  format: yaml
  label: Airbrake Projects API
  slug: airbrake-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-projects-api-openapi.yml
- filename: airbrake-sessions-api-openapi.yml
  format: yaml
  label: Airbrake Sessions API
  slug: airbrake-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-sessions-api-openapi.yml
- filename: airbrake-source-maps-api-openapi.yml
  format: yaml
  label: Airbrake Source Maps API
  slug: airbrake-source-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-source-maps-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@airbrake.io"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airbrake.io
  spf: true
hosts:
- cert_expires: Sep 14 05:18:46 2026 GMT
  host: www.airbrake.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: docs.airbrake.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.airbrake.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airbrake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airbrake, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airbrake
provider_slug: airbrake
slug: airbrake-domain-security
source_filename: airbrake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airbrake.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:18:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.airbrake.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: api.airbrake.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: airbrake.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@airbrake.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/security/airbrake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Error Monitoring
- Application Performance Monitoring
- Observability
- DevOps
- Logging
- Exception Tracking
---
