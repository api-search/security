---
api_specs:
- filename: bugsnag-data-access-openapi.yml
  format: yaml
  label: Bugsnag Data Access API
  slug: data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-data-access-openapi.yml
- filename: bugsnag-error-reporting-openapi.yml
  format: yaml
  label: Bugsnag Error Reporting API
  slug: error-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-error-reporting-openapi.yml
- filename: bugsnag-session-tracking-openapi.yml
  format: yaml
  label: Bugsnag Session Tracking API
  slug: session-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-session-tracking-openapi.yml
- filename: bugsnag-build-openapi.yml
  format: yaml
  label: Bugsnag Build API
  slug: build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-build-openapi.yml
- filename: bugsnag-trace-openapi.yml
  format: yaml
  label: Bugsnag Trace API
  slug: trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-trace-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bugsnag.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: docs.bugsnag.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: api.bugsnag.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: notify.bugsnag.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bugsnag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bugsnag, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: bugsnag
provider_slug: bugsnag
slug: bugsnag-domain-security
source_filename: bugsnag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.bugsnag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.bugsnag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: notify.bugsnag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bugsnag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/security/bugsnag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
