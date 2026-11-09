---
api_specs:
- filename: audit-domains-account-api-openapi.yml
  format: yaml
  label: audit.domains Account API
  slug: audit-domains-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-account-api-openapi.yml
- filename: audit-domains-appraisals-api-openapi.yml
  format: yaml
  label: audit.domains Appraisals API
  slug: audit-domains-appraisals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-appraisals-api-openapi.yml
- filename: audit-domains-bulk-api-openapi.yml
  format: yaml
  label: audit.domains Bulk API
  slug: audit-domains-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-bulk-api-openapi.yml
- filename: audit-domains-machine-api-openapi.yml
  format: yaml
  label: audit.domains Machine API
  slug: audit-domains-machine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-machine-api-openapi.yml
- filename: audit-domains-sales-api-openapi.yml
  format: yaml
  label: audit.domains Sales API
  slug: audit-domains-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-sales-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audit.domains
  spf: true
hosts:
- cert_expires: Jan 12 08:32:02 2027 GMT
  host: audit.domains
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audit Domains Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for audit.domains, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: audit.domains
provider_slug: audit-domains
slug: audit-domains-domain-security
source_filename: audit-domains-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audit.domains\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 08:32:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: audit.domains\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/audit-domains/security/audit-domains-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Domain
- Valuation
- Analytics
- Portfolio
---
