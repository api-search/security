---
api_specs:
- filename: globaldatabase-com-autocomplete-api-openapi.yml
  format: yaml
  label: Global Database Autocomplete API
  slug: globaldatabase-com-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-autocomplete-api-openapi.yml
- filename: globaldatabase-com-company-by-linkedin-api-openapi.yml
  format: yaml
  label: Global Database Company By Linkedin API
  slug: globaldatabase-com-company-by-linkedin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-company-by-linkedin-api-openapi.yml
- filename: globaldatabase-com-company-by-url-api-openapi.yml
  format: yaml
  label: Global Database Company By Url API
  slug: globaldatabase-com-company-by-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-company-by-url-api-openapi.yml
- filename: globaldatabase-com-company-details-api-openapi.yml
  format: yaml
  label: Global Database Company Details API
  slug: globaldatabase-com-company-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-company-details-api-openapi.yml
- filename: globaldatabase-com-company-financials-api-openapi.yml
  format: yaml
  label: Global Database Company Financials API
  slug: globaldatabase-com-company-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-company-financials-api-openapi.yml
- filename: globaldatabase-com-company-ownership-api-openapi.yml
  format: yaml
  label: Global Database Company Ownership API
  slug: globaldatabase-com-company-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-company-ownership-api-openapi.yml
- filename: globaldatabase-com-fastapi-api-openapi.yml
  format: yaml
  label: Global Database Fast API
  slug: globaldatabase-com-fastapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-fastapi-api-openapi.yml
- filename: globaldatabase-com-health-api-openapi.yml
  format: yaml
  label: Global Database Health API
  slug: globaldatabase-com-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-health-api-openapi.yml
- filename: globaldatabase-com-nomenclature-api-openapi.yml
  format: yaml
  label: Global Database Nomenclature API
  slug: globaldatabase-com-nomenclature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-nomenclature-api-openapi.yml
- filename: globaldatabase-com-oauth-api-openapi.yml
  format: yaml
  label: Global Database OAuth API
  slug: globaldatabase-com-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-oauth-api-openapi.yml
- filename: globaldatabase-com-playground-api-openapi.yml
  format: yaml
  label: Global Database Playground API
  slug: globaldatabase-com-playground-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-playground-api-openapi.yml
- filename: globaldatabase-com-prospecting-api-openapi.yml
  format: yaml
  label: Global Database Prospecting API
  slug: globaldatabase-com-prospecting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-prospecting-api-openapi.yml
- filename: globaldatabase-com-verify-token-api-openapi.yml
  format: yaml
  label: Global Database Verify Token API
  slug: globaldatabase-com-verify-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-verify-token-api-openapi.yml
- filename: globaldatabase-com-well-known-api-openapi.yml
  format: yaml
  label: Global Database .well Known API
  slug: globaldatabase-com-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-well-known-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: globaldatabase.com
  spf: true
hosts:
- cert_expires: Nov 17 22:00:16 2026 GMT
  host: globaldatabase.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Globaldatabase Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Global Database, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Global Database
provider_slug: globaldatabase-com
slug: globaldatabase-com-domain-security
source_filename: globaldatabase-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: globaldatabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 22:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: globaldatabase.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/security/globaldatabase-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Company Data
- KYB
- Compliance
- Business Verification
- Beneficial Ownership
- Finance
- Credit Risk
- Data Enrichment
- Prospecting
- Webhook
- MCP
- AI Agents
- United Kingdom
---
