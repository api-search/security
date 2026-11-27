---
api_specs:
- filename: measure-sh-alerts-api-openapi.yml
  format: yaml
  label: Measure Alerts API
  slug: measure-sh-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-alerts-api-openapi.yml
- filename: measure-sh-apps-api-openapi.yml
  format: yaml
  label: Measure Apps API
  slug: measure-sh-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-apps-api-openapi.yml
- filename: measure-sh-auth-api-openapi.yml
  format: yaml
  label: Measure Auth API
  slug: measure-sh-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-auth-api-openapi.yml
- filename: measure-sh-bug-reports-api-openapi.yml
  format: yaml
  label: Measure Bug Reports API
  slug: measure-sh-bug-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-bug-reports-api-openapi.yml
- filename: measure-sh-builds-api-openapi.yml
  format: yaml
  label: Measure Builds API
  slug: measure-sh-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-builds-api-openapi.yml
- filename: measure-sh-config-api-openapi.yml
  format: yaml
  label: Measure Config API
  slug: measure-sh-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-config-api-openapi.yml
- filename: measure-sh-devices-api-openapi.yml
  format: yaml
  label: Measure Devices API
  slug: measure-sh-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-devices-api-openapi.yml
- filename: measure-sh-errors-api-openapi.yml
  format: yaml
  label: Measure Errors API
  slug: measure-sh-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-errors-api-openapi.yml
- filename: measure-sh-events-api-openapi.yml
  format: yaml
  label: Measure Events API
  slug: measure-sh-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-events-api-openapi.yml
- filename: measure-sh-funnels-api-openapi.yml
  format: yaml
  label: Measure Funnels API
  slug: measure-sh-funnels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-funnels-api-openapi.yml
- filename: measure-sh-memory-api-openapi.yml
  format: yaml
  label: Measure Memory API
  slug: measure-sh-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-memory-api-openapi.yml
- filename: measure-sh-network-requests-api-openapi.yml
  format: yaml
  label: Measure Network Requests API
  slug: measure-sh-network-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-network-requests-api-openapi.yml
- filename: measure-sh-prefs-api-openapi.yml
  format: yaml
  label: Measure Prefs API
  slug: measure-sh-prefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-prefs-api-openapi.yml
- filename: measure-sh-profiles-api-openapi.yml
  format: yaml
  label: Measure Profiles API
  slug: measure-sh-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-profiles-api-openapi.yml
- filename: measure-sh-sessions-api-openapi.yml
  format: yaml
  label: Measure Sessions API
  slug: measure-sh-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-sessions-api-openapi.yml
- filename: measure-sh-teams-api-openapi.yml
  format: yaml
  label: Measure Teams API
  slug: measure-sh-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-teams-api-openapi.yml
- filename: measure-sh-traces-api-openapi.yml
  format: yaml
  label: Measure Traces API
  slug: measure-sh-traces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-traces-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:infra-alerts@measure.sh"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: measure.sh
  spf: true
hosts:
- cert_expires: Jan 22 17:17:42 2027 GMT
  host: measure.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Measure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Measure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Measure
provider_slug: measure-sh
slug: measure-sh-domain-security
source_filename: measure-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: measure.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 17:17:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: measure.sh\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:infra-alerts@measure.sh\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/measure-sh/security/measure-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Mobile
- Monitoring
- Open Source
- Crash Reporting
- Observability
---
