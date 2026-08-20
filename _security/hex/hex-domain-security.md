---
api_specs:
- filename: hex-cells-api-openapi.yml
  format: yaml
  label: Hex Cells API
  slug: hex-cells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-cells-api-openapi.yml
- filename: hex-collections-api-openapi.yml
  format: yaml
  label: Hex Collections API
  slug: hex-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-collections-api-openapi.yml
- filename: hex-context-api-openapi.yml
  format: yaml
  label: Hex Context API
  slug: hex-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-context-api-openapi.yml
- filename: hex-data-connections-api-openapi.yml
  format: yaml
  label: Hex Data Connections API
  slug: hex-data-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-data-connections-api-openapi.yml
- filename: hex-embedding-api-openapi.yml
  format: yaml
  label: Hex Embedding API
  slug: hex-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-embedding-api-openapi.yml
- filename: hex-groups-api-openapi.yml
  format: yaml
  label: Hex Groups API
  slug: hex-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-groups-api-openapi.yml
- filename: hex-guides-api-openapi.yml
  format: yaml
  label: Hex Guides API
  slug: hex-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-guides-api-openapi.yml
- filename: hex-projects-api-openapi.yml
  format: yaml
  label: Hex Projects API
  slug: hex-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-projects-api-openapi.yml
- filename: hex-semantic-projects-models-api-openapi.yml
  format: yaml
  label: Hex Semantic (projects|models) API
  slug: hex-semantic-projects-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-semantic-projects-models-api-openapi.yml
- filename: hex-threads-api-openapi.yml
  format: yaml
  label: Hex Threads API
  slug: hex-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-threads-api-openapi.yml
- filename: hex-users-api-openapi.yml
  format: yaml
  label: Hex Users API
  slug: hex-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa-reports@hex.tech"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hex.tech
  spf: true
hosts:
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
name: Hex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hex
provider_slug: hex
slug: hex-domain-security
source_filename: hex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.hex.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:14:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.hex.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:18:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hex.tech\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa-reports@hex.tech\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/security/hex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Data Science
- Notebooks
- Business Intelligence
- Data Apps
- Artificial Intelligence
- Agents
- Semantic Layer
- Developer Tools
---
