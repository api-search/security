---
api_specs:
- filename: honeycomb-api-openapi.yml
  format: yaml
  label: Honeycomb API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-api-openapi.yml
- filename: honeycomb-events-api-openapi.yml
  format: yaml
  label: Honeycomb Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-events-api-openapi.yml
- filename: honeycomb-queries-api-openapi.yml
  format: yaml
  label: Honeycomb Queries API
  slug: queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-queries-api-openapi.yml
- filename: honeycomb-slos-api-openapi.yml
  format: yaml
  label: Honeycomb SLOs API
  slug: slos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-slos-api-openapi.yml
- filename: honeycomb-datasets-api-openapi.yml
  format: yaml
  label: Honeycomb Datasets API
  slug: datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-datasets-api-openapi.yml
- filename: honeycomb-boards-api-openapi.yml
  format: yaml
  label: Honeycomb Boards API
  slug: boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-boards-api-openapi.yml
- filename: honeycomb-markers-api-openapi.yml
  format: yaml
  label: Honeycomb Markers API
  slug: markers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-markers-api-openapi.yml
- filename: honeycomb-triggers-api-openapi.yml
  format: yaml
  label: Honeycomb Triggers API
  slug: triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-triggers-api-openapi.yml
- filename: honeycomb-environments-api-openapi.yml
  format: yaml
  label: Honeycomb Environments API
  slug: environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-environments-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:support@honeycomb.io"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: honeycomb.io
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api-docs.honeycomb.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.honeycomb.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Honeycomb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for honeycomb, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: honeycomb
provider_slug: honeycomb
slug: honeycomb-domain-security
source_filename: honeycomb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-docs.honeycomb.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.honeycomb.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: honeycomb.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:support@honeycomb.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/security/honeycomb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
