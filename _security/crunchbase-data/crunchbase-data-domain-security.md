---
api_specs:
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Entity Lookup API
  slug: crunchbase-data-entity-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Search API
  slug: crunchbase-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Autocomplete API
  slug: crunchbase-data-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Deleted Entities API
  slug: crunchbase-data-deleted-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
description: ''
domains:
- domain: crunchbase.com
  note: TLS/DNS posture (TLS version, HSTS, DNSSEC, CAA, SPF, DMARC) was not live probed in this run; values should be confirmed with a live probe during reconciliation. The API strictly requires HTTPS.
hosts:
- host: api.crunchbase.com
  https: true
  note: HTTPS required for all API calls; non-HTTPS requests are rejected with HTTP 426.
- host: data.crunchbase.com
  https: true
  note: Developer documentation host.
- host: www.crunchbase.com
  https: true
  note: Primary product and marketing website.
kind: domain-security
layout: security
method: modeled
name: Crunchbase Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crunchbase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Crunchbase
provider_slug: crunchbase-data
slug: crunchbase-data-domain-security
source_filename: crunchbase-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: modeled\nsource: apis.yml + OpenAPI hosts (not live-probed in this run)\nhosts:\n- host: api.crunchbase.com\n  https: true\n  note: HTTPS required for all API calls; non-HTTPS requests are rejected with HTTP 426.\n- host: data.crunchbase.com\n  https: true\n  note: Developer documentation host.\n- host: www.crunchbase.com\n  https: true\n  note: Primary product and marketing website.\ndomains:\n- domain: crunchbase.com\n  note: >-\n    TLS/DNS posture (TLS version, HSTS, DNSSEC, CAA, SPF, DMARC) was not live\n    probed in this run; values should be confirmed with a live probe during\n    reconciliation. The API strictly requires HTTPS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/security/crunchbase-data-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company Data
- Web Intelligence
- Funding Data
- Firmographics
- B2B Data
- Investor Data
- Reference Data
- Fortune 1000
---
