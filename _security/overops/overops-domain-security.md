---
api_specs:
- filename: overops-alerts-api-openapi.yml
  format: yaml
  label: Overops Alerts API
  slug: overops-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-alerts-api-openapi.yml
- filename: overops-categories-api-openapi.yml
  format: yaml
  label: Overops Categories API
  slug: overops-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-categories-api-openapi.yml
- filename: overops-code-redaction-api-openapi.yml
  format: yaml
  label: Overops Code Redaction API
  slug: overops-code-redaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-code-redaction-api-openapi.yml
- filename: overops-data-redaction-api-openapi.yml
  format: yaml
  label: Overops Data Redaction API
  slug: overops-data-redaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-data-redaction-api-openapi.yml
- filename: overops-entry-points-api-openapi.yml
  format: yaml
  label: Overops Entry Points API
  slug: overops-entry-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-entry-points-api-openapi.yml
- filename: overops-environment-management-api-openapi.yml
  format: yaml
  label: Overops Environment Management API
  slug: overops-environment-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-environment-management-api-openapi.yml
- filename: overops-events-api-openapi.yml
  format: yaml
  label: Overops Events API
  slug: overops-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-events-api-openapi.yml
- filename: overops-general-api-openapi.yml
  format: yaml
  label: Overops General API
  slug: overops-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-general-api-openapi.yml
- filename: overops-labels-api-openapi.yml
  format: yaml
  label: Overops Labels API
  slug: overops-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-labels-api-openapi.yml
- filename: overops-publish-metrics-api-openapi.yml
  format: yaml
  label: Overops Publish Metrics API
  slug: overops-publish-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-publish-metrics-api-openapi.yml
- filename: overops-system-metrics-api-openapi.yml
  format: yaml
  label: Overops System Metrics API
  slug: overops-system-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-system-metrics-api-openapi.yml
- filename: overops-team-management-api-openapi.yml
  format: yaml
  label: Overops Team Management API
  slug: overops-team-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-team-management-api-openapi.yml
- filename: overops-timers-api-openapi.yml
  format: yaml
  label: Overops Timers API
  slug: overops-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-timers-api-openapi.yml
- filename: overops-udfs-api-openapi.yml
  format: yaml
  label: Overops UDFs API
  slug: overops-udfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-udfs-api-openapi.yml
- filename: overops-view-metrics-api-openapi.yml
  format: yaml
  label: Overops View Metrics API
  slug: overops-view-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-view-metrics-api-openapi.yml
- filename: overops-views-api-openapi.yml
  format: yaml
  label: Overops Views API
  slug: overops-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-views-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: overops.com
  spf: true
hosts:
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: api.overops.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Overops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overops, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Overops
provider_slug: overops
slug: overops-domain-security
source_filename: overops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.overops.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: overops.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/security/overops-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Observability
- Reliability
- Error Monitoring
- Application Performance
- Java
- DevOps
- Code Quality
---
