---
api_specs:
- filename: internetdata-io-lookup-api-openapi.yml
  format: yaml
  label: InternetData Lookup API
  slug: internetdata-io-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-lookup-api-openapi.yml
- filename: internetdata-io-entitlement-api-openapi.yml
  format: yaml
  label: InternetData Entitlement API
  slug: internetdata-io-entitlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-entitlement-api-openapi.yml
- filename: internetdata-io-account-api-openapi.yml
  format: yaml
  label: InternetData Account API
  slug: internetdata-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-account-api-openapi.yml
- filename: internetdata-io-api-keys-api-openapi.yml
  format: yaml
  label: InternetData API keys API
  slug: internetdata-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-api-keys-api-openapi.yml
- filename: internetdata-io-authorization-api-openapi.yml
  format: yaml
  label: InternetData Authorization API
  slug: internetdata-io-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-authorization-api-openapi.yml
- filename: internetdata-io-database-api-openapi.yml
  format: yaml
  label: InternetData Database API
  slug: internetdata-io-database-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-database-api-openapi.yml
- filename: internetdata-io-database-v2-api-openapi.yml
  format: yaml
  label: InternetData Database v2 API
  slug: internetdata-io-database-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-database-v2-api-openapi.yml
- filename: internetdata-io-organization-api-openapi.yml
  format: yaml
  label: InternetData Organization API
  slug: internetdata-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-organization-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: internetdata.io
  spf: true
hosts:
- cert_expires: Feb  6 13:57:13 2027 GMT
  host: internetdata.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InternetData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InternetData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InternetData
provider_slug: internetdata-io
slug: internetdata-io-domain-security
source_filename: internetdata-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: internetdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 13:57:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: internetdata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/internetdata-io/security/internetdata-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IP Intelligence
- Data Licensing
- Geolocation
- Network Security
---
