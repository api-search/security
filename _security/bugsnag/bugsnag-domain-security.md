---
api_specs:
- filename: bugsnag-builds-api-openapi.yml
  format: yaml
  label: bugsnag Builds API
  slug: bugsnag-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-builds-api-openapi.yml
- filename: bugsnag-collaborators-api-openapi.yml
  format: yaml
  label: bugsnag Collaborators API
  slug: bugsnag-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-collaborators-api-openapi.yml
- filename: bugsnag-comments-api-openapi.yml
  format: yaml
  label: bugsnag Comments API
  slug: bugsnag-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-comments-api-openapi.yml
- filename: bugsnag-currentuser-api-openapi.yml
  format: yaml
  label: bugsnag CurrentUser API
  slug: bugsnag-currentuser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-currentuser-api-openapi.yml
- filename: bugsnag-errors-api-openapi.yml
  format: yaml
  label: bugsnag Errors API
  slug: bugsnag-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-errors-api-openapi.yml
- filename: bugsnag-eventfields-api-openapi.yml
  format: yaml
  label: bugsnag EventFields API
  slug: bugsnag-eventfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-eventfields-api-openapi.yml
- filename: bugsnag-events-api-openapi.yml
  format: yaml
  label: bugsnag Events API
  slug: bugsnag-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-events-api-openapi.yml
- filename: bugsnag-notifications-api-openapi.yml
  format: yaml
  label: bugsnag Notifications API
  slug: bugsnag-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-notifications-api-openapi.yml
- filename: bugsnag-organizations-api-openapi.yml
  format: yaml
  label: bugsnag Organizations API
  slug: bugsnag-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-organizations-api-openapi.yml
- filename: bugsnag-pivots-api-openapi.yml
  format: yaml
  label: bugsnag Pivots API
  slug: bugsnag-pivots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-pivots-api-openapi.yml
- filename: bugsnag-projects-api-openapi.yml
  format: yaml
  label: bugsnag Projects API
  slug: bugsnag-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-projects-api-openapi.yml
- filename: bugsnag-releases-api-openapi.yml
  format: yaml
  label: bugsnag Releases API
  slug: bugsnag-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-releases-api-openapi.yml
- filename: bugsnag-sessions-api-openapi.yml
  format: yaml
  label: bugsnag Sessions API
  slug: bugsnag-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-sessions-api-openapi.yml
- filename: bugsnag-stability-api-openapi.yml
  format: yaml
  label: bugsnag Stability API
  slug: bugsnag-stability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-stability-api-openapi.yml
- filename: bugsnag-traces-api-openapi.yml
  format: yaml
  label: bugsnag Traces API
  slug: bugsnag-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-traces-api-openapi.yml
- filename: bugsnag-trends-api-openapi.yml
  format: yaml
  label: bugsnag Trends API
  slug: bugsnag-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-trends-api-openapi.yml
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
overview: 'Domain security posture for Bugsnag, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bugsnag
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
