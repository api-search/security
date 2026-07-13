---
api_specs:
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Sink Consumers API
  slug: sequin-io-sink-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Postgres Databases API
  slug: sequin-io-postgres-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin HTTP Endpoints API
  slug: sequin-io-http-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Backfills API
  slug: sequin-io-backfills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Stream Pull API
  slug: sequin-io-stream-pull-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sequinstream.com
  spf: false
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: sequinstream.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: api.sequinstream.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sequin Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequin, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Sequin
provider_slug: sequin-io
slug: sequin-io-domain-security
source_filename: sequin-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sequinstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.sequinstream.com\n  https: false\ndomains:\n- domain: sequinstream.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/security/sequin-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Change Data Capture
- CDC
- Postgres
- Streaming
- Open Source
- Data Pipeline
---
