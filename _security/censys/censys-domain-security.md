---
api_specs:
- filename: censys-account-management-api-openapi.yml
  format: yaml
  label: Censys Account Management API
  slug: censys-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-account-management-api-openapi.yml
- filename: censys-adversary-investigation-api-openapi.yml
  format: yaml
  label: Censys Adversary Investigation API
  slug: censys-adversary-investigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-adversary-investigation-api-openapi.yml
- filename: censys-asset-graphs-api-openapi.yml
  format: yaml
  label: Censys Asset Graphs API
  slug: censys-asset-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-asset-graphs-api-openapi.yml
- filename: censys-assets-api-openapi.yml
  format: yaml
  label: Censys Assets API
  slug: censys-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-assets-api-openapi.yml
- filename: censys-collections-api-openapi.yml
  format: yaml
  label: Censys Collections API
  slug: censys-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-collections-api-openapi.yml
- filename: censys-excluded-assets-api-openapi.yml
  format: yaml
  label: Censys Excluded Assets API
  slug: censys-excluded-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-excluded-assets-api-openapi.yml
- filename: censys-global-data-api-openapi.yml
  format: yaml
  label: Censys Global Data API
  slug: censys-global-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-global-data-api-openapi.yml
- filename: censys-graph-executions-api-openapi.yml
  format: yaml
  label: Censys Graph Executions API
  slug: censys-graph-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-graph-executions-api-openapi.yml
- filename: censys-risks-api-openapi.yml
  format: yaml
  label: Censys Risks API
  slug: censys-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-risks-api-openapi.yml
- filename: censys-seeds-api-openapi.yml
  format: yaml
  label: Censys Seeds API
  slug: censys-seeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-seeds-api-openapi.yml
- filename: censys-shards-api-openapi.yml
  format: yaml
  label: Censys Shards API
  slug: censys-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-shards-api-openapi.yml
- filename: censys-supply-chain-intelligence-api-openapi.yml
  format: yaml
  label: Censys Supply Chain Intelligence API
  slug: censys-supply-chain-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-supply-chain-intelligence-api-openapi.yml
- filename: censys-tags-and-comments-api-openapi.yml
  format: yaml
  label: Censys Tags and Comments API
  slug: censys-tags-and-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-tags-and-comments-api-openapi.yml
- filename: censys-threat-hunting-api-openapi.yml
  format: yaml
  label: Censys Threat Hunting API
  slug: censys-threat-hunting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-threat-hunting-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild ";"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: censys.com
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild ";"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: censys.io
  spf: true
hosts:
- cert_expires: Sep 16 15:32:30 2026 GMT
  host: censys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 14:24:25 2026 GMT
  host: platform.censys.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 22:43:03 2026 GMT
  host: docs.censys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Censys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Censys, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Censys
provider_slug: censys
slug: censys-domain-security
source_filename: censys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: censys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:32:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.censys.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:24:25 2026 GMT\n  hsts: null\n- host: docs.censys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 22:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: censys.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \";\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: censys.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \";\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com;\
  \ cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/security/censys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Internet Intelligence
- Attack Surface Management
- Threat Hunting
- Cyber Threat Intelligence
- OSINT
- Internet Scanning
- Certificates
- Asset Discovery
---
