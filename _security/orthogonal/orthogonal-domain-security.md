---
api_specs:
- filename: orthogonal-account-api-openapi.yml
  format: yaml
  label: Orthogonal Account API
  slug: orthogonal-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-account-api-openapi.yml
- filename: orthogonal-discovery-api-openapi.yml
  format: yaml
  label: Orthogonal Discovery API
  slug: orthogonal-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-discovery-api-openapi.yml
- filename: orthogonal-run-api-openapi.yml
  format: yaml
  label: Orthogonal Run API
  slug: orthogonal-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-run-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: orthogonal.com
  spf: false
hosts:
- cert_expires: Aug 26 17:27:25 2026 GMT
  host: www.orthogonal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orthogonal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orthogonal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Orthogonal
provider_slug: orthogonal
slug: orthogonal-domain-security
source_filename: orthogonal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orthogonal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:27:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orthogonal.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/security/orthogonal-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI Agents
- API Discovery
- API Marketplace
- Agent Payments
- MCP
- Data Enrichment
- Crypto
- Stablecoins
---
