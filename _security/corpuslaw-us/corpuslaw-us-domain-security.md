---
api_specs:
- filename: corpuslaw-us-account-api-openapi.yml
  format: yaml
  label: Corpus Account API
  slug: corpuslaw-us-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-account-api-openapi.yml
- filename: corpuslaw-us-browse-api-openapi.yml
  format: yaml
  label: Corpus Browse API
  slug: corpuslaw-us-browse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-browse-api-openapi.yml
- filename: corpuslaw-us-coverage-api-openapi.yml
  format: yaml
  label: Corpus Coverage API
  slug: corpuslaw-us-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-coverage-api-openapi.yml
- filename: corpuslaw-us-formation-api-openapi.yml
  format: yaml
  label: Corpus Formation API
  slug: corpuslaw-us-formation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-formation-api-openapi.yml
- filename: corpuslaw-us-general-api-openapi.yml
  format: yaml
  label: Corpus General API
  slug: corpuslaw-us-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-general-api-openapi.yml
- filename: corpuslaw-us-gis-api-openapi.yml
  format: yaml
  label: Corpus GIS API
  slug: corpuslaw-us-gis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-gis-api-openapi.yml
- filename: corpuslaw-us-search-api-openapi.yml
  format: yaml
  label: Corpus Search API
  slug: corpuslaw-us-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpuslaw-us/openapi/corpuslaw-us-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: corpuslaw.us
  spf: true
hosts:
- cert_expires: Jan 30 12:39:47 2027 GMT
  host: corpuslaw.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corpus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corpus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Corpus
provider_slug: corpuslaw-us
slug: corpuslaw-us-domain-security
source_filename: corpuslaw-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corpuslaw.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 12:39:47 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: corpuslaw.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/corpuslaw-us/security/corpuslaw-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Law
- Business Formation
- LLC
- Compliance
- MCP
- AI Agents
---
