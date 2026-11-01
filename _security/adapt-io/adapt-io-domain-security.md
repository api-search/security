---
api_specs:
- filename: adapt-io-account-api-openapi.yml
  format: yaml
  label: Adapt Account API
  slug: adapt-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-account-api-openapi.yml
- filename: adapt-io-company-api-openapi.yml
  format: yaml
  label: Adapt Company API
  slug: adapt-io-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-company-api-openapi.yml
- filename: adapt-io-contact-api-openapi.yml
  format: yaml
  label: Adapt Contact API
  slug: adapt-io-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-contact-api-openapi.yml
- filename: adapt-io-contribution-api-openapi.yml
  format: yaml
  label: Adapt Contribution API
  slug: adapt-io-contribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-contribution-api-openapi.yml
- filename: adapt-io-email-api-openapi.yml
  format: yaml
  label: Adapt Email API
  slug: adapt-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-email-api-openapi.yml
- filename: adapt-io-emailid-api-openapi.yml
  format: yaml
  label: Adapt Emailid API
  slug: adapt-io-emailid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-emailid-api-openapi.yml
- filename: adapt-io-filter-api-openapi.yml
  format: yaml
  label: Adapt Filter API
  slug: adapt-io-filter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-filter-api-openapi.yml
- filename: adapt-io-health-api-openapi.yml
  format: yaml
  label: Adapt Health API
  slug: adapt-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-health-api-openapi.yml
- filename: adapt-io-webhooks-api-openapi.yml
  format: yaml
  label: Adapt Webhooks API
  slug: adapt-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adapt.io
  spf: true
hosts:
- cert_expires: Sep 19 13:02:08 2026 GMT
  host: www.adapt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 13:02:08 2026 GMT
  host: api.adapt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Adapt Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adapt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adapt
provider_slug: adapt-io
slug: adapt-io-domain-security
source_filename: adapt-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adapt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:02:08 2026 GMT\n  hsts: false\n- host: api.adapt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:02:08 2026 GMT\n  hsts: null\ndomains:\n- domain: adapt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/adapt-io/security/adapt-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- B2B Data
- Contact Data
- Company Data
- Lead Intelligence
- Sales Intelligence
- Sales Acceleration
- Data Enrichment
- Prospecting
- Lead Generation
- Email Finder
- Account Based Marketing
- CRM Enrichment
- Marketing
- Sales
---
