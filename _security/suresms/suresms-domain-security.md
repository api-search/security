---
api_specs:
- filename: suresms-authenticate-api-openapi.yml
  format: yaml
  label: SureSMS Authenticate API
  slug: suresms-authenticate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-authenticate-api-openapi.yml
- filename: suresms-coverage-api-openapi.yml
  format: yaml
  label: SureSMS Coverage API
  slug: suresms-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-coverage-api-openapi.yml
- filename: suresms-message-api-openapi.yml
  format: yaml
  label: SureSMS Message API
  slug: suresms-message-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-message-api-openapi.yml
- filename: suresms-messagestatus-api-openapi.yml
  format: yaml
  label: SureSMS Message Status API
  slug: suresms-messagestatus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-messagestatus-api-openapi.yml
- filename: suresms-price-api-openapi.yml
  format: yaml
  label: SureSMS Price API
  slug: suresms-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-price-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: suresms.com
  spf: true
hosts:
- cert_expires: Feb  9 05:57:01 2027 GMT
  host: suresms.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SureSMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SureSMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SureSMS
provider_slug: suresms
slug: suresms-domain-security
source_filename: suresms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suresms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 05:57:01 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: suresms.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/suresms/security/suresms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SMS Gateway
- Communications Platform
- Industry Solutions
- Integration Services
---
