---
api_specs:
- filename: databazaar-io-account-api-openapi.yml
  format: yaml
  label: DataBazaar Account API
  slug: databazaar-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-account-api-openapi.yml
- filename: databazaar-io-agent-api-openapi.yml
  format: yaml
  label: DataBazaar Agent API
  slug: databazaar-io-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-agent-api-openapi.yml
- filename: databazaar-io-bounty-submissions-api-openapi.yml
  format: yaml
  label: DataBazaar Bounty Submissions API
  slug: databazaar-io-bounty-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-bounty-submissions-api-openapi.yml
- filename: databazaar-io-categories-api-openapi.yml
  format: yaml
  label: DataBazaar Categories API
  slug: databazaar-io-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-categories-api-openapi.yml
- filename: databazaar-io-datasets-api-openapi.yml
  format: yaml
  label: DataBazaar Datasets API
  slug: databazaar-io-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-datasets-api-openapi.yml
- filename: databazaar-io-listings-api-openapi.yml
  format: yaml
  label: DataBazaar Listings API
  slug: databazaar-io-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-listings-api-openapi.yml
- filename: databazaar-io-purchases-api-openapi.yml
  format: yaml
  label: DataBazaar Purchases API
  slug: databazaar-io-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-purchases-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: databazaar.io
  spf: false
hosts:
- cert_expires: Dec 27 16:59:06 2026 GMT
  host: databazaar.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Databazaar Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataBazaar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: DataBazaar
provider_slug: databazaar-io
slug: databazaar-io-domain-security
source_filename: databazaar-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: databazaar.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 16:59:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: databazaar.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/databazaar-io/security/databazaar-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Marketplace
- AI Agents
- Datasets
- Marketplace
- Agent-Native
---
