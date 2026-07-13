---
api_specs:
- filename: openapi-derefed.json
  format: json
  label: Sentry API
  slug: sentry-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Events and Issues API
  slug: sentry-events-and-issues-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Organizations API
  slug: sentry-organizations-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Projects API
  slug: sentry-projects-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Teams API
  slug: sentry-teams-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Releases API
  slug: sentry-releases-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Alerts API
  slug: sentry-alerts-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Crons API
  slug: sentry-crons-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Dashboards API
  slug: sentry-dashboards-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Discover API
  slug: sentry-discover-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Environments API
  slug: sentry-environments-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Explore API
  slug: sentry-explore-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Integration Platform API
  slug: sentry-integration-platform-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Integrations API
  slug: sentry-integrations-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Mobile Builds API
  slug: sentry-mobile-builds-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Monitors API
  slug: sentry-monitors-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Prevent API
  slug: sentry-prevent-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Replays API
  slug: sentry-replays-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry SCIM API
  slug: sentry-scim-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Seer API
  slug: sentry-seer-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Users API
  slug: sentry-users-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@sentry.io"
  - 0 issue "letsencrypt.org"
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
name: Sentry System Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentry, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sentry
provider_slug: sentry-system
slug: sentry-system-domain-security
source_filename: sentry-system-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sentry.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sentry.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:42:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sentry.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@sentry.io\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/security/sentry-system-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
---
