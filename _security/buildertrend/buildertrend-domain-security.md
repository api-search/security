---
api_specs:
- filename: buildertrend-authentication-api-openapi.yml
  format: yaml
  label: Buildertrend Authentication API
  slug: buildertrend-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-authentication-api-openapi.yml
- filename: buildertrend-jobs-api-openapi.yml
  format: yaml
  label: Buildertrend Jobs API
  slug: buildertrend-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-jobs-api-openapi.yml
- filename: buildertrend-tasks-api-openapi.yml
  format: yaml
  label: Buildertrend Tasks API
  slug: buildertrend-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-tasks-api-openapi.yml
- filename: buildertrend-utility-api-openapi.yml
  format: yaml
  label: Buildertrend Utility API
  slug: buildertrend-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildertrend/openapi/buildertrend-utility-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:domain@buildertrend.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: buildertrend.com
  spf: true
hosts:
- cert_expires: Jan 16 09:34:37 2027 GMT
  host: buildertrend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buildertrend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildertrend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Buildertrend
provider_slug: buildertrend
slug: buildertrend-domain-security
source_filename: buildertrend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildertrend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 09:34:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buildertrend.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:domain@buildertrend.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/buildertrend/security/buildertrend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Construction
- Construction Management
- Residential Construction
- Home Builders
- Remodeling
- Specialty Contractors
- Project Management
- Job Costing
- Estimating
- Scheduling
- CRM
- Proposals
- Change Orders
- Purchase Orders
- Invoicing
- Client Portal
- Subcontractor Portal
- Mobile App
- Software-as-a-Service
- Vertical SaaS
- Construction Technology
---
