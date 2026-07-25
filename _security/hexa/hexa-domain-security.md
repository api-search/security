---
api_specs:
- filename: hexa-cells-api-openapi.yml
  format: yaml
  label: Hex Cells API
  slug: hexa-cells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-cells-api-openapi.yml
- filename: hexa-collections-api-openapi.yml
  format: yaml
  label: Hex Collections API
  slug: hexa-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-collections-api-openapi.yml
- filename: hexa-data-connections-api-openapi.yml
  format: yaml
  label: Hex Data Connections API
  slug: hexa-data-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-data-connections-api-openapi.yml
- filename: hexa-embedding-api-openapi.yml
  format: yaml
  label: Hex Embedding API
  slug: hexa-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-embedding-api-openapi.yml
- filename: hexa-groups-api-openapi.yml
  format: yaml
  label: Hex Groups API
  slug: hexa-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-groups-api-openapi.yml
- filename: hexa-guides-api-openapi.yml
  format: yaml
  label: Hex Guides API
  slug: hexa-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-guides-api-openapi.yml
- filename: hexa-projects-api-openapi.yml
  format: yaml
  label: Hex Projects API
  slug: hexa-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-projects-api-openapi.yml
- filename: hexa-semantic-projects-models-api-openapi.yml
  format: yaml
  label: Hex Semantic (projects|models) API
  slug: hexa-semantic-projects-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-semantic-projects-models-api-openapi.yml
- filename: hexa-users-api-openapi.yml
  format: yaml
  label: Hex Users API
  slug: hexa-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa-reports@hex.tech"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hex.tech
  spf: true
hosts:
- cert_expires: Sep 14 06:51:44 2026 GMT
  host: hex.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 00:14:59 2026 GMT
  host: learn.hex.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 06:18:18 2026 GMT
  host: app.hex.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hex
provider_slug: hexa
slug: hexa-domain-security
source_filename: hexa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hex.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:51:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.hex.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:14:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.hex.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:18:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hex.tech\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa-reports@hex.tech\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/security/hexa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Collaboration
- Data
- Notebooks
---
