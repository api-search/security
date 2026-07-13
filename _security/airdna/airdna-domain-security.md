---
api_specs:
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Market Search
  slug: market-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Market Stats
  slug: market-stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Property/Listing Data
  slug: property-listing-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Rentalizer Estimates
  slug: rentalizer-estimates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Comps
  slug: comps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airdna.co
  spf: true
hosts:
- cert_expires: Sep 23 22:18:31 2026 GMT
  host: www.airdna.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 22:18:31 2026 GMT
  host: docs.airdna.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: api.airdna.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airdna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirDNA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AirDNA
provider_slug: airdna
slug: airdna-domain-security
source_filename: airdna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airdna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:18:31 2026 GMT\n  hsts: false\n- host: docs.airdna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:18:31 2026 GMT\n  hsts: false\n- host: api.airdna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: airdna.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/security/airdna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Short-Term Rental
- Vacation Rental
- Market Data
- Real Estate
- Analytics
---
