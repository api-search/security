---
api_specs:
- filename: consumer-financial-protection-bureau-aggregations-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau Aggregations API
  slug: consumer-financial-protection-bureau-aggregations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/consumer-financial-protection-bureau-aggregations-api-openapi.yml
- filename: consumer-financial-protection-bureau-csv-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau CSV API
  slug: consumer-financial-protection-bureau-csv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/consumer-financial-protection-bureau-csv-api-openapi.yml
- filename: consumer-financial-protection-bureau-filers-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau Filers API
  slug: consumer-financial-protection-bureau-filers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/consumer-financial-protection-bureau-filers-api-openapi.yml
- filename: consumer-financial-protection-bureau-geo-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau Geo API
  slug: consumer-financial-protection-bureau-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/consumer-financial-protection-bureau-geo-api-openapi.yml
- filename: consumer-financial-protection-bureau-institutions-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau Institutions API
  slug: consumer-financial-protection-bureau-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/consumer-financial-protection-bureau-institutions-api-openapi.yml
- filename: consumer-financial-protection-bureau-search-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau Search API
  slug: consumer-financial-protection-bureau-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/consumer-financial-protection-bureau-search-api-openapi.yml
- filename: consumer-financial-protection-bureau-trends-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau Trends API
  slug: consumer-financial-protection-bureau-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/consumer-financial-protection-bureau-trends-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: consumerfinance.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cfpb.gov
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.consumerfinance.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: ffiec.cfpb.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Consumer Financial Protection Bureau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consumer Financial Protection Bureau, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Consumer Financial Protection Bureau
provider_slug: consumer-financial-protection-bureau
slug: consumer-financial-protection-bureau-domain-security
source_filename: consumer-financial-protection-bureau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.consumerfinance.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: ffiec.cfpb.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: consumerfinance.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cfpb.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/security/consumer-financial-protection-bureau-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Banking
- Complaints
- Consumer Protection
- Federal Government
- Financial Services
- HMDA
- Mortgages
- Open Data
---
