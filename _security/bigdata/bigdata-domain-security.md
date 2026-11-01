---
api_specs:
- filename: bigdata-analyst-estimates-api-openapi.yml
  format: yaml
  label: RavenPack Analyst Estimates API
  slug: bigdata-analyst-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-analyst-estimates-api-openapi.yml
- filename: bigdata-company-events-api-openapi.yml
  format: yaml
  label: RavenPack Company & Events API
  slug: bigdata-company-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-company-events-api-openapi.yml
- filename: bigdata-financials-ratios-api-openapi.yml
  format: yaml
  label: RavenPack Financials & Ratios API
  slug: bigdata-financials-ratios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-financials-ratios-api-openapi.yml
- filename: bigdata-fixed-income-api-openapi.yml
  format: yaml
  label: RavenPack Fixed Income API
  slug: bigdata-fixed-income-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-fixed-income-api-openapi.yml
- filename: bigdata-fund-holdings-api-openapi.yml
  format: yaml
  label: RavenPack Fund Holdings API
  slug: bigdata-fund-holdings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-fund-holdings-api-openapi.yml
- filename: bigdata-market-data-api-openapi.yml
  format: yaml
  label: RavenPack Market Data API
  slug: bigdata-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-market-data-api-openapi.yml
- filename: bigdata-private-markets-api-openapi.yml
  format: yaml
  label: RavenPack Private Markets API
  slug: bigdata-private-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-private-markets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@ravenpack.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bigdata.com
  spf: true
hosts:
- cert_expires: Dec 13 12:59:05 2026 GMT
  host: bigdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bigdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RavenPack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: RavenPack
provider_slug: bigdata
slug: bigdata-domain-security
source_filename: bigdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 12:59:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bigdata.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@ravenpack.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bigdata/security/bigdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Artificial Intelligence
- Data Analytics
- Market Insights
---
