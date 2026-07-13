---
api_specs:
- filename: sentry-api-openapi.yml
  format: yaml
  label: Sentry Error Monitoring API
  slug: sentry-error-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/openapi/sentry-api-openapi.yml
- filename: sentry-webhooks-asyncapi.yml
  format: yaml
  label: Sentry Integration Platform API
  slug: sentry-integration-platform-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/asyncapi/sentry-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@sentry.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sentry.io
  spf: true
hosts:
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: sentry.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:42:45 2026 GMT
  host: docs.sentry.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sentry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentry, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sentry
provider_slug: sentry
slug: sentry-domain-security
source_filename: sentry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sentry.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sentry.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:42:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sentry.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@sentry.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/security/sentry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Error Monitoring
- Debugging
- Observability
- Application Performance Management
- Developer Tools
---
