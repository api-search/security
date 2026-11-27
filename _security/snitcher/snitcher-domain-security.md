---
api_specs:
- filename: snitcher-contacts-api-openapi.yml
  format: yaml
  label: Snitcher Contacts API
  slug: snitcher-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-contacts-api-openapi.yml
- filename: snitcher-custom-field-values-api-openapi.yml
  format: yaml
  label: Snitcher Custom Field Values API
  slug: snitcher-custom-field-values-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-custom-field-values-api-openapi.yml
- filename: snitcher-custom-fields-api-openapi.yml
  format: yaml
  label: Snitcher Custom Fields API
  slug: snitcher-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-custom-fields-api-openapi.yml
- filename: snitcher-organisations-api-openapi.yml
  format: yaml
  label: Snitcher Organisations API
  slug: snitcher-organisations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-organisations-api-openapi.yml
- filename: snitcher-segments-api-openapi.yml
  format: yaml
  label: Snitcher Segments API
  slug: snitcher-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-segments-api-openapi.yml
- filename: snitcher-sessions-api-openapi.yml
  format: yaml
  label: Snitcher Sessions API
  slug: snitcher-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-sessions-api-openapi.yml
- filename: snitcher-user-api-openapi.yml
  format: yaml
  label: Snitcher User API
  slug: snitcher-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-user-api-openapi.yml
- filename: snitcher-workspaces-api-openapi.yml
  format: yaml
  label: Snitcher Workspaces API
  slug: snitcher-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snitcher.com
  spf: true
hosts:
- cert_expires: Feb 10 12:37:09 2027 GMT
  host: snitcher.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Snitcher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snitcher, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Snitcher
provider_slug: snitcher
slug: snitcher-domain-security
source_filename: snitcher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snitcher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 12:37:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: snitcher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/snitcher/security/snitcher-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Visitor Intelligence
- B2B SaaS
- Lead Generation
- Marketing Automation
---
