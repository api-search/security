---
api_specs:
- filename: emitrr-actions-api-openapi.yml
  format: yaml
  label: Emitrr Actions API
  slug: emitrr-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emitrr/openapi/emitrr-actions-api-openapi.yml
- filename: emitrr-branches-api-openapi.yml
  format: yaml
  label: Emitrr Branches API
  slug: emitrr-branches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emitrr/openapi/emitrr-branches-api-openapi.yml
- filename: emitrr-core-api-openapi.yml
  format: yaml
  label: Emitrr Core API
  slug: emitrr-core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emitrr/openapi/emitrr-core-api-openapi.yml
- filename: emitrr-filters-api-openapi.yml
  format: yaml
  label: Emitrr Filters API
  slug: emitrr-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emitrr/openapi/emitrr-filters-api-openapi.yml
- filename: emitrr-health-api-openapi.yml
  format: yaml
  label: Emitrr Health API
  slug: emitrr-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emitrr/openapi/emitrr-health-api-openapi.yml
- filename: emitrr-triggers-api-openapi.yml
  format: yaml
  label: Emitrr Triggers API
  slug: emitrr-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emitrr/openapi/emitrr-triggers-api-openapi.yml
- filename: emitrr-workflows-api-openapi.yml
  format: yaml
  label: Emitrr Workflows API
  slug: emitrr-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emitrr/openapi/emitrr-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emitrr.com
  spf: true
hosts:
- cert_expires: Dec 26 09:44:54 2026 GMT
  host: emitrr.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Emitrr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emitrr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Emitrr
provider_slug: emitrr
slug: emitrr-domain-security
source_filename: emitrr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emitrr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 09:44:54 2026 GMT\n  hsts: false\ndomains:\n- domain: emitrr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/emitrr/security/emitrr-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Healthcare
- AI
- Communication
- Messaging
- SaaS
---
