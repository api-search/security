---
api_specs:
- filename: dynatrace-entities-api-openapi.yml
  format: yaml
  label: Dynatrace Entities API
  slug: dynatrace-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-entities-api-openapi.yml
- filename: dynatrace-environments-api-openapi.yml
  format: yaml
  label: Dynatrace Environments API
  slug: dynatrace-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-environments-api-openapi.yml
- filename: dynatrace-events-api-openapi.yml
  format: yaml
  label: Dynatrace Events API
  slug: dynatrace-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-events-api-openapi.yml
- filename: dynatrace-groups-api-openapi.yml
  format: yaml
  label: Dynatrace Groups API
  slug: dynatrace-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-groups-api-openapi.yml
- filename: dynatrace-logs-api-openapi.yml
  format: yaml
  label: Dynatrace Logs API
  slug: dynatrace-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-logs-api-openapi.yml
- filename: dynatrace-metrics-api-openapi.yml
  format: yaml
  label: Dynatrace Metrics API
  slug: dynatrace-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-metrics-api-openapi.yml
- filename: dynatrace-permissions-api-openapi.yml
  format: yaml
  label: Dynatrace Permissions API
  slug: dynatrace-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-permissions-api-openapi.yml
- filename: dynatrace-problems-api-openapi.yml
  format: yaml
  label: Dynatrace Problems API
  slug: dynatrace-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-problems-api-openapi.yml
- filename: dynatrace-users-api-openapi.yml
  format: yaml
  label: Dynatrace Users API
  slug: dynatrace-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dynatrace.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: www.dynatrace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: docs.dynatrace.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: mysampleenv.live.dynatrace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dynatrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynatrace, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dynatrace
provider_slug: dynatrace
slug: dynatrace-domain-security
source_filename: dynatrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dynatrace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dynatrace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: mysampleenv.live.dynatrace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dynatrace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/security/dynatrace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
---
