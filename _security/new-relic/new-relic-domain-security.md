---
api_specs:
- filename: new-relic-openapi.yml
  format: yaml
  label: New Relic REST API v2
  slug: new-relic-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-openapi.yml
- filename: new-relic-metric-api-openapi.yml
  format: yaml
  label: New Relic Metric API
  slug: new-relic-metric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-metric-api-openapi.yml
- filename: new-relic-event-api-openapi.yml
  format: yaml
  label: New Relic Event API
  slug: new-relic-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-event-api-openapi.yml
- filename: new-relic-log-api-openapi.yml
  format: yaml
  label: New Relic Log API
  slug: new-relic-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-log-api-openapi.yml
- filename: new-relic-trace-api-openapi.yml
  format: yaml
  label: New Relic Trace API
  slug: new-relic-trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-trace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: newrelic.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: newrelic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 27 06:13:45 2026 GMT
  host: developer.newrelic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 11:53:43 2026 GMT
  host: docs.newrelic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: New Relic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New Relic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: New Relic
provider_slug: new-relic
slug: new-relic-domain-security
source_filename: new-relic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newrelic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.newrelic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 06:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.newrelic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 11:53:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: newrelic.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/security/new-relic-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
---
