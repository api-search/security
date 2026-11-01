---
api_specs:
- filename: leadmagic-io-ads-data-api-openapi.yml
  format: yaml
  label: leadmagic-io Ads Data API
  slug: leadmagic-io-ads-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-ads-data-api-openapi.yml
- filename: leadmagic-io-analytics-api-openapi.yml
  format: yaml
  label: leadmagic-io Analytics API
  slug: leadmagic-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-analytics-api-openapi.yml
- filename: leadmagic-io-batch-api-openapi.yml
  format: yaml
  label: leadmagic-io Batch API
  slug: leadmagic-io-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-batch-api-openapi.yml
- filename: leadmagic-io-bulk-jobs-api-openapi.yml
  format: yaml
  label: leadmagic-io Bulk Jobs API
  slug: leadmagic-io-bulk-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-bulk-jobs-api-openapi.yml
- filename: leadmagic-io-company-data-api-openapi.yml
  format: yaml
  label: leadmagic-io Company Data API
  slug: leadmagic-io-company-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-company-data-api-openapi.yml
- filename: leadmagic-io-cost-control-api-openapi.yml
  format: yaml
  label: leadmagic-io Cost Control API
  slug: leadmagic-io-cost-control-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-cost-control-api-openapi.yml
- filename: leadmagic-io-credits-api-openapi.yml
  format: yaml
  label: leadmagic-io Credits API
  slug: leadmagic-io-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-credits-api-openapi.yml
- filename: leadmagic-io-jobs-data-api-openapi.yml
  format: yaml
  label: leadmagic-io Jobs Data API
  slug: leadmagic-io-jobs-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-jobs-data-api-openapi.yml
- filename: leadmagic-io-people-enrichment-api-openapi.yml
  format: yaml
  label: leadmagic-io People Enrichment API
  slug: leadmagic-io-people-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadmagic-io/openapi/leadmagic-io-people-enrichment-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: leadmagic.io
  spf: true
hosts:
- cert_expires: Dec 18 23:43:54 2026 GMT
  host: leadmagic.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Leadmagic Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for leadmagic-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: leadmagic-io
provider_slug: leadmagic-io
slug: leadmagic-io-domain-security
source_filename: leadmagic-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadmagic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: leadmagic.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/leadmagic-io/security/leadmagic-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- B2B
- Data Enrichment
- Lead Generation
- Email Verification
- Company Intelligence
---
