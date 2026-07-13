---
api_specs:
- filename: 6sense-company-identification-api-openapi.yml
  format: yaml
  label: 6sense Company Identification API
  slug: 6sense-company-identification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-identification-api-openapi.yml
- filename: 6sense-company-firmographics-api-openapi.yml
  format: yaml
  label: 6sense Company Firmographics API
  slug: 6sense-company-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-firmographics-api-openapi.yml
- filename: 6sense-lead-scoring-api-openapi.yml
  format: yaml
  label: 6sense Lead Scoring API
  slug: 6sense-lead-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-lead-scoring-api-openapi.yml
- filename: 6sense-lead-scoring-firmographics-api-openapi.yml
  format: yaml
  label: 6sense Lead Scoring And Firmographics API
  slug: 6sense-lead-scoring-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-lead-scoring-firmographics-api-openapi.yml
- filename: 6sense-people-enrichment-api-openapi.yml
  format: yaml
  label: 6sense People Enrichment API
  slug: 6sense-people-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-enrichment-api-openapi.yml
- filename: 6sense-people-search-api-openapi.yml
  format: yaml
  label: 6sense People Search API
  slug: 6sense-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 6sense.com
  spf: true
hosts:
- cert_expires: Sep 13 19:06:08 2026 GMT
  host: 6sense.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.6sense.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: epsilon.6sense.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 6Sense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 6sense, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 6sense
provider_slug: 6sense
slug: 6sense-domain-security
source_filename: 6sense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 6sense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:06:08 2026 GMT\n  hsts: null\n- host: api.6sense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\n- host: epsilon.6sense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 6sense.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/security/6sense-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- ABM
- Account-Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- AI
- Marketing Technology
---
