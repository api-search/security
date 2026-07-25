---
api_specs:
- filename: s2-dev-access-tokens-api-openapi.yml
  format: yaml
  label: S2 Dev access-tokens API
  slug: s2-dev-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/openapi/s2-dev-access-tokens-api-openapi.yml
- filename: s2-dev-basins-api-openapi.yml
  format: yaml
  label: S2 Dev basins API
  slug: s2-dev-basins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/openapi/s2-dev-basins-api-openapi.yml
- filename: s2-dev-locations-api-openapi.yml
  format: yaml
  label: S2 Dev locations API
  slug: s2-dev-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/openapi/s2-dev-locations-api-openapi.yml
- filename: s2-dev-metrics-api-openapi.yml
  format: yaml
  label: S2 Dev metrics API
  slug: s2-dev-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/openapi/s2-dev-metrics-api-openapi.yml
- filename: s2-dev-records-api-openapi.yml
  format: yaml
  label: S2 Dev records API
  slug: s2-dev-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/openapi/s2-dev-records-api-openapi.yml
- filename: s2-dev-streams-api-openapi.yml
  format: yaml
  label: S2 Dev streams API
  slug: s2-dev-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/openapi/s2-dev-streams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: s2.dev
  spf: true
hosts:
- cert_expires: Sep 21 13:28:56 2026 GMT
  host: a.s2.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: S2 Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for S2 Dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: S2 Dev
provider_slug: s2-dev
slug: s2-dev-domain-security
source_filename: s2-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a.s2.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:28:56 2026 GMT\n  hsts: null\ndomains:\n- domain: s2.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/security/s2-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Streaming
- Real-Time
- Event Streaming
- Durable Storage
- Message Streaming
- Data Feeds
- Observability
- Developer Tools
- Infrastructure
---
