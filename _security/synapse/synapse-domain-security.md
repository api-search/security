---
api_specs:
- filename: synapse-federation-api-openapi.yml
  format: yaml
  label: Synapse Federation API
  slug: synapse-federation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-federation-api-openapi.yml
- filename: synapse-media-api-openapi.yml
  format: yaml
  label: Synapse Media API
  slug: synapse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-media-api-openapi.yml
- filename: synapse-registration-api-openapi.yml
  format: yaml
  label: Synapse Registration API
  slug: synapse-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-registration-api-openapi.yml
- filename: synapse-reports-api-openapi.yml
  format: yaml
  label: Synapse Reports API
  slug: synapse-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-reports-api-openapi.yml
- filename: synapse-rooms-api-openapi.yml
  format: yaml
  label: Synapse Rooms API
  slug: synapse-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-rooms-api-openapi.yml
- filename: synapse-server-api-openapi.yml
  format: yaml
  label: Synapse Server API
  slug: synapse-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-server-api-openapi.yml
- filename: synapse-statistics-api-openapi.yml
  format: yaml
  label: Synapse Statistics API
  slug: synapse-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-statistics-api-openapi.yml
- filename: synapse-users-api-openapi.yml
  format: yaml
  label: Synapse Users API
  slug: synapse-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/openapi/synapse-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: matrix.org
  spf: true
hosts:
- cert_expires: Oct  6 19:46:11 2026 GMT
  host: spec.matrix.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synapse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synapse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synapse
provider_slug: synapse
slug: synapse-domain-security
source_filename: synapse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spec.matrix.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:46:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: matrix.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synapse/refs/heads/main/security/synapse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat
- Collaboration
- Decentralized
- Federation
- Matrix
- Messaging
- Open-Source
- Real-Time
---
