---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Rollbar REST API
  slug: rollbar-rest-api
  spec_type: OpenAPI
  url: https://explorer.docs.rollbar.com/
- filename: rollbar-deployment-api-openapi.yml
  format: yaml
  label: Rollbar Deployment API
  slug: rollbar-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-deployment-api-openapi.yml
- filename: rollbar-metrics-api-openapi.yml
  format: yaml
  label: Rollbar Metrics API
  slug: rollbar-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-metrics-api-openapi.yml
- filename: rollbar-rql-api-openapi.yml
  format: yaml
  label: Rollbar RQL API
  slug: rollbar-rql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-rql-api-openapi.yml
- filename: rollbar-webhooks-asyncapi.yml
  format: yaml
  label: Rollbar Webhooks
  slug: rollbar-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/asyncapi/rollbar-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rollbar.com
  spf: true
hosts:
- cert_expires: Aug 11 20:14:09 2026 GMT
  host: rollbar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: explorer.docs.rollbar.com
  https: false
- cert_expires: Oct  2 13:37:34 2026 GMT
  host: docs.rollbar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rollbar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rollbar, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rollbar
provider_slug: rollbar
slug: rollbar-domain-security
source_filename: rollbar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rollbar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 20:14:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: explorer.docs.rollbar.com\n  https: false\n- host: docs.rollbar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:37:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rollbar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/security/rollbar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Error Tracking
- Monitoring
- Debugging
- DevOps
- Application Performance
---
