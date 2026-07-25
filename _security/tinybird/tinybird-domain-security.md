---
api_specs:
- filename: tinybird-analyze-api-openapi.yml
  format: yaml
  label: Tinybird Analyze API
  slug: tinybird-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-analyze-api-openapi.yml
- filename: tinybird-data-sources-api-openapi.yml
  format: yaml
  label: Tinybird Data Sources API
  slug: tinybird-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-data-sources-api-openapi.yml
- filename: tinybird-environment-variables-api-openapi.yml
  format: yaml
  label: Tinybird Environment Variables API
  slug: tinybird-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-environment-variables-api-openapi.yml
- filename: tinybird-events-api-openapi.yml
  format: yaml
  label: Tinybird Events API
  slug: tinybird-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-events-api-openapi.yml
- filename: tinybird-jobs-api-openapi.yml
  format: yaml
  label: Tinybird Jobs API
  slug: tinybird-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-jobs-api-openapi.yml
- filename: tinybird-organizations-api-openapi.yml
  format: yaml
  label: Tinybird Organizations API
  slug: tinybird-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-organizations-api-openapi.yml
- filename: tinybird-pipes-api-openapi.yml
  format: yaml
  label: Tinybird Pipes API
  slug: tinybird-pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-pipes-api-openapi.yml
- filename: tinybird-query-api-openapi.yml
  format: yaml
  label: Tinybird Query API
  slug: tinybird-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-query-api-openapi.yml
- filename: tinybird-sink-pipes-api-openapi.yml
  format: yaml
  label: Tinybird Sink Pipes API
  slug: tinybird-sink-pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-sink-pipes-api-openapi.yml
- filename: tinybird-tokens-api-openapi.yml
  format: yaml
  label: Tinybird Tokens API
  slug: tinybird-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/openapi/tinybird-tokens-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tinybird.co
  spf: true
hosts:
- cert_expires: Aug 30 16:45:20 2026 GMT
  host: www.tinybird.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 12:37:04 2026 GMT
  host: api.tinybird.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:33:32 2026 GMT
  host: api.us-east.tinybird.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tinybird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tinybird, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tinybird
provider_slug: tinybird
slug: tinybird-domain-security
source_filename: tinybird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tinybird.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 16:45:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tinybird.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:37:04 2026 GMT\n  hsts: null\n- host: api.us-east.tinybird.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:33:32 2026 GMT\n  hsts: null\ndomains:\n- domain: tinybird.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tinybird/refs/heads/main/security/tinybird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Data
- Real-Time
- SQL
- Streaming
---
