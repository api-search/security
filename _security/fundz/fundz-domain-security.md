---
api_specs:
- filename: fundz-acquisitions-api-openapi.yml
  format: yaml
  label: Fundz Acquisitions API
  slug: fundz-acquisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-acquisitions-api-openapi.yml
- filename: fundz-agreements-api-openapi.yml
  format: yaml
  label: Fundz Agreements API
  slug: fundz-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-agreements-api-openapi.yml
- filename: fundz-crowdfundings-api-openapi.yml
  format: yaml
  label: Fundz Crowdfundings API
  slug: fundz-crowdfundings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-crowdfundings-api-openapi.yml
- filename: fundz-executives-api-openapi.yml
  format: yaml
  label: Fundz Executives API
  slug: fundz-executives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-executives-api-openapi.yml
- filename: fundz-fundings-api-openapi.yml
  format: yaml
  label: Fundz Fundings API
  slug: fundz-fundings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-fundings-api-openapi.yml
- filename: fundz-products-api-openapi.yml
  format: yaml
  label: Fundz Products API
  slug: fundz-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/openapi/fundz-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fundz.net
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.fundz.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.fundz.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fundz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fundz, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fundz
provider_slug: fundz
slug: fundz-domain-security
source_filename: fundz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fundz.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: api.fundz.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fundz.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/security/fundz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Intelligence
- Funding
- Private Markets
- Mergers and Acquisitions
- SEC Filings
- Signals
- Sales Intelligence
- MCP
- Agents
---
