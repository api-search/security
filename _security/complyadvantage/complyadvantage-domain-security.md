---
api_specs:
- filename: complyadvantage-mesh-api-openapi.json
  format: json
  label: ComplyAdvantage Mesh Platform API
  slug: complyadvantage-mesh-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-mesh-api-openapi.json
- filename: complyadvantage-case-management-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Case Management API
  slug: complyadvantage-case-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-case-management-api-openapi.yml
- filename: complyadvantage-monitored-searches-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Monitored Searches API
  slug: complyadvantage-monitored-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-monitored-searches-api-openapi.yml
- filename: complyadvantage-searches-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Searches API
  slug: complyadvantage-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-searches-api-openapi.yml
- filename: complyadvantage-users-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Users API
  slug: complyadvantage-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: complyadvantage.com
  spf: true
hosts:
- cert_expires: Nov 11 09:34:28 2026 GMT
  host: complyadvantage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 13:11:48 2026 GMT
  host: docs.mesh.complyadvantage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:37:38 2026 GMT
  host: api.mesh.complyadvantage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Complyadvantage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ComplyAdvantage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ComplyAdvantage
provider_slug: complyadvantage
slug: complyadvantage-domain-security
source_filename: complyadvantage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: complyadvantage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 09:34:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mesh.complyadvantage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 13:11:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mesh.complyadvantage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:37:38 2026 GMT\n  hsts: null\ndomains:\n- domain: complyadvantage.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/security/complyadvantage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Anti-Money Laundering
- AML
- Fraud Detection
- Sanctions Screening
- Compliance
- PEP Screening
- Adverse Media
- KYC
- Watchlist
- Transaction Monitoring
- Financial Crime
- RegTech
---
