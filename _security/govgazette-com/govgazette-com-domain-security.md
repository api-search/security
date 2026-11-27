---
api_specs:
- filename: govgazette-com-documents-api-openapi.yml
  format: yaml
  label: GovGazette Documents API
  slug: govgazette-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-documents-api-openapi.yml
- filename: govgazette-com-exclusions-api-openapi.yml
  format: yaml
  label: GovGazette Exclusions API
  slug: govgazette-com-exclusions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-exclusions-api-openapi.yml
- filename: govgazette-com-freshness-api-openapi.yml
  format: yaml
  label: GovGazette Freshness API
  slug: govgazette-com-freshness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-freshness-api-openapi.yml
- filename: govgazette-com-govgazette-api-openapi.yml
  format: yaml
  label: GovGazette Gov Gazette API
  slug: govgazette-com-govgazette-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-govgazette-api-openapi.yml
- filename: govgazette-com-match-api-openapi.yml
  format: yaml
  label: GovGazette Match API
  slug: govgazette-com-match-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-match-api-openapi.yml
- filename: govgazette-com-opportunities-api-openapi.yml
  format: yaml
  label: GovGazette Opportunities API
  slug: govgazette-com-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-opportunities-api-openapi.yml
- filename: govgazette-com-records-api-openapi.yml
  format: yaml
  label: GovGazette Records API
  slug: govgazette-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-records-api-openapi.yml
- filename: govgazette-com-search-api-openapi.yml
  format: yaml
  label: GovGazette Search API
  slug: govgazette-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-search-api-openapi.yml
- filename: govgazette-com-status-api-openapi.yml
  format: yaml
  label: GovGazette Status API
  slug: govgazette-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govgazette-com/openapi/govgazette-com-status-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: govgazette.com
  spf: true
hosts:
- cert_expires: Dec 26 04:55:01 2026 GMT
  host: govgazette.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GovGazette Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GovGazette, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: GovGazette
provider_slug: govgazette-com
slug: govgazette-com-domain-security
source_filename: govgazette-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govgazette.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 04:55:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: govgazette.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/govgazette-com/security/govgazette-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Government
- Procurement
- Contracts
- Data
---
