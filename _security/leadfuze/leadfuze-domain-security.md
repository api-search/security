---
api_specs:
- filename: leadfuze-email-verification-api-openapi.yml
  format: yaml
  label: LeadFuze Email verification API
  slug: leadfuze-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-email-verification-api-openapi.yml
- filename: leadfuze-enrichment-api-openapi.yml
  format: yaml
  label: LeadFuze Enrichment API
  slug: leadfuze-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-enrichment-api-openapi.yml
- filename: leadfuze-identity-resolution-pixel-api-openapi.yml
  format: yaml
  label: LeadFuze Identity Resolution Pixel API
  slug: leadfuze-identity-resolution-pixel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-identity-resolution-pixel-api-openapi.yml
- filename: leadfuze-integrations-api-openapi.yml
  format: yaml
  label: LeadFuze Integrations API
  slug: leadfuze-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-integrations-api-openapi.yml
- filename: leadfuze-intent-data-api-openapi.yml
  format: yaml
  label: LeadFuze Intent data API
  slug: leadfuze-intent-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-intent-data-api-openapi.yml
- filename: leadfuze-lead-database-api-openapi.yml
  format: yaml
  label: LeadFuze Lead database API
  slug: leadfuze-lead-database-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-lead-database-api-openapi.yml
- filename: leadfuze-phone-validation-api-openapi.yml
  format: yaml
  label: LeadFuze Phone validation API
  slug: leadfuze-phone-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-phone-validation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leadfuze.com
  spf: true
hosts:
- cert_expires: Jan  2 06:46:49 2027 GMT
  host: leadfuze.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LeadFuze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeadFuze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LeadFuze
provider_slug: leadfuze
slug: leadfuze-domain-security
source_filename: leadfuze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadfuze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 06:46:49 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: leadfuze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leadfuze/security/leadfuze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Lead Generation
- Sales
- Marketing
- Data Enrichment
- B2B
---
