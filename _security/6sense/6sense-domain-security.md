---
api_specs:
- filename: 6sense-company-api-openapi.yml
  format: yaml
  label: 6sense Company API
  slug: 6sense-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-api-openapi.yml
- filename: 6sense-enrichment-api-openapi.yml
  format: yaml
  label: 6sense Enrichment API
  slug: 6sense-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-enrichment-api-openapi.yml
- filename: 6sense-people-api-openapi.yml
  format: yaml
  label: 6sense People API
  slug: 6sense-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-api-openapi.yml
- filename: 6sense-scoring-api-openapi.yml
  format: yaml
  label: 6sense Scoring API
  slug: 6sense-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-scoring-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
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
kind: domain-security
layout: security
method: probed
name: 6Sense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 6sense, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 6sense
provider_slug: 6sense
slug: 6sense-domain-security
source_filename: 6sense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 6sense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:06:08 2026 GMT\n  hsts: null\n- host: api.6sense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 6sense.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/security/6sense-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Account Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- Artificial Intelligence
- Marketing Technology
---
