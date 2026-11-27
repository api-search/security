---
api_specs:
- filename: hollyhr-com-org-units-api-openapi.yml
  format: yaml
  label: HollyHR Org Units API
  slug: hollyhr-com-org-units-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-org-units-api-openapi.yml
- filename: hollyhr-com-people-api-openapi.yml
  format: yaml
  label: HollyHR People API
  slug: hollyhr-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-people-api-openapi.yml
- filename: hollyhr-com-time-off-api-openapi.yml
  format: yaml
  label: HollyHR Time Off API
  slug: hollyhr-com-time-off-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-time-off-api-openapi.yml
- filename: hollyhr-com-webhooks-api-openapi.yml
  format: yaml
  label: HollyHR Webhooks API
  slug: hollyhr-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-webhooks-api-openapi.yml
- filename: hollyhr-com-working-patterns-api-openapi.yml
  format: yaml
  label: HollyHR Working Patterns API
  slug: hollyhr-com-working-patterns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-working-patterns-api-openapi.yml
- filename: hollyhr-com-custom-fields-api-openapi.yml
  format: yaml
  label: HollyHR Custom Fields API
  slug: hollyhr-com-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-custom-fields-api-openapi.yml
- filename: hollyhr-com-documents-api-openapi.yml
  format: yaml
  label: HollyHR Documents API
  slug: hollyhr-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-documents-api-openapi.yml
- filename: hollyhr-com-employers-api-openapi.yml
  format: yaml
  label: HollyHR Employers API
  slug: hollyhr-com-employers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-employers-api-openapi.yml
- filename: hollyhr-com-exports-api-openapi.yml
  format: yaml
  label: HollyHR Exports API
  slug: hollyhr-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-exports-api-openapi.yml
- filename: hollyhr-com-integrations-api-openapi.yml
  format: yaml
  label: HollyHR Integrations API
  slug: hollyhr-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-integrations-api-openapi.yml
- filename: hollyhr-com-meta-api-openapi.yml
  format: yaml
  label: HollyHR Meta API
  slug: hollyhr-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-meta-api-openapi.yml
- filename: hollyhr-com-organisation-api-openapi.yml
  format: yaml
  label: HollyHR Organisation API
  slug: hollyhr-com-organisation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-organisation-api-openapi.yml
- filename: hollyhr-com-provider-mappings-api-openapi.yml
  format: yaml
  label: HollyHR Provider Mappings API
  slug: hollyhr-com-provider-mappings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-provider-mappings-api-openapi.yml
- filename: hollyhr-com-reference-data-api-openapi.yml
  format: yaml
  label: HollyHR Reference Data API
  slug: hollyhr-com-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hollyhr-com/openapi/hollyhr-com-reference-data-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hollyhr.com
  spf: true
hosts:
- cert_expires: Dec 23 13:50:52 2026 GMT
  host: hollyhr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HollyHR Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HollyHR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HollyHR
provider_slug: hollyhr-com
slug: hollyhr-com-domain-security
source_filename: hollyhr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hollyhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 13:50:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hollyhr.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hollyhr-com/security/hollyhr-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human Resources
- Software-as-a-Service
- United Kingdom
- Small Business
- Payroll
---
