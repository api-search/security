---
api_specs:
- filename: datocapital-com-account-api-openapi.yml
  format: yaml
  label: Dato Capital Account API
  slug: datocapital-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-account-api-openapi.yml
- filename: datocapital-com-companies-api-openapi.yml
  format: yaml
  label: Dato Capital Companies API
  slug: datocapital-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-companies-api-openapi.yml
- filename: datocapital-com-filings-api-openapi.yml
  format: yaml
  label: Dato Capital Filings API
  slug: datocapital-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-filings-api-openapi.yml
- filename: datocapital-com-health-api-openapi.yml
  format: yaml
  label: Dato Capital Health API
  slug: datocapital-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-health-api-openapi.yml
- filename: datocapital-com-individuals-api-openapi.yml
  format: yaml
  label: Dato Capital Individuals API
  slug: datocapital-com-individuals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-individuals-api-openapi.yml
- filename: datocapital-com-reference-api-openapi.yml
  format: yaml
  label: Dato Capital Reference API
  slug: datocapital-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-reference-api-openapi.yml
- filename: datocapital-com-suggest-api-openapi.yml
  format: yaml
  label: Dato Capital Suggest API
  slug: datocapital-com-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-suggest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: datocapital.com
  spf: true
hosts:
- cert_expires: Dec  6 04:07:52 2026 GMT
  host: datocapital.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datocapital Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dato Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dato Capital
provider_slug: datocapital-com
slug: datocapital-com-domain-security
source_filename: datocapital-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datocapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 04:07:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datocapital.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/datocapital-com/security/datocapital-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Search
- Compliance
- Due Diligence
---
