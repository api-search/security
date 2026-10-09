---
api_specs:
- filename: monid-api-keys-api-openapi.yml
  format: yaml
  label: Monid API Keys API
  slug: monid-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-api-keys-api-openapi.yml
- filename: monid-auth-api-openapi.yml
  format: yaml
  label: Monid Auth API
  slug: monid-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-auth-api-openapi.yml
- filename: monid-controls-api-openapi.yml
  format: yaml
  label: Monid Controls API
  slug: monid-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-controls-api-openapi.yml
- filename: monid-discover-api-openapi.yml
  format: yaml
  label: Monid Discover API
  slug: monid-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-discover-api-openapi.yml
- filename: monid-endpoints-api-openapi.yml
  format: yaml
  label: Monid Endpoints API
  slug: monid-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-endpoints-api-openapi.yml
- filename: monid-inspect-api-openapi.yml
  format: yaml
  label: Monid Inspect API
  slug: monid-inspect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-inspect-api-openapi.yml
- filename: monid-public-registry-api-openapi.yml
  format: yaml
  label: Monid Public Registry API
  slug: monid-public-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-public-registry-api-openapi.yml
- filename: monid-resources-api-openapi.yml
  format: yaml
  label: Monid Resources API
  slug: monid-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-resources-api-openapi.yml
- filename: monid-runs-api-openapi.yml
  format: yaml
  label: Monid Runs API
  slug: monid-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-runs-api-openapi.yml
- filename: monid-wallet-api-openapi.yml
  format: yaml
  label: Monid Wallet API
  slug: monid-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-wallet-api-openapi.yml
- filename: monid-identities-api-openapi.yml
  format: yaml
  label: Monid Identities API
  slug: monid-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-identities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: monid.ai
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: monid.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.monid.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Monid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Monid
provider_slug: monid
slug: monid-domain-security
source_filename: monid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: false\n- host: api.monid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monid.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/security/monid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Agents
- MCP
- Tools
- Data
- API Marketplace
---
