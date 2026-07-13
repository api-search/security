---
api_specs:
- filename: keen-event-collection-api-openapi.yml
  format: yaml
  label: Keen Event Collection API
  slug: event-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-event-collection-api-openapi.yml
- filename: keen-query-api-openapi.yml
  format: yaml
  label: Keen Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-query-api-openapi.yml
- filename: keen-cached-queries-api-openapi.yml
  format: yaml
  label: Keen Cached Queries API
  slug: cached-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-cached-queries-api-openapi.yml
- filename: keen-saved-queries-api-openapi.yml
  format: yaml
  label: Keen Saved Queries API
  slug: saved-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-saved-queries-api-openapi.yml
- filename: keen-data-extraction-api-openapi.yml
  format: yaml
  label: Keen Data Extraction API
  slug: data-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-data-extraction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: keen.io
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: keen.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.keen.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Keen
provider_slug: keen
slug: keen-domain-security
source_filename: keen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keen.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.keen.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: keen.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/security/keen-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Analytics
- Custom Events
- Data Collection
- Embedded Analytics
- Event Analytics
---
