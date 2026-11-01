---
api_specs:
- filename: foundational-auth-api-openapi.yml
  format: yaml
  label: Foundational Auth API
  slug: foundational-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-auth-api-openapi.yml
- filename: foundational-lineage-api-openapi.yml
  format: yaml
  label: Foundational Lineage API
  slug: foundational-lineage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-lineage-api-openapi.yml
- filename: foundational-manual-lineage-api-openapi.yml
  format: yaml
  label: Foundational Manual Lineage API
  slug: foundational-manual-lineage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-manual-lineage-api-openapi.yml
- filename: foundational-monitors-api-openapi.yml
  format: yaml
  label: Foundational Monitors API
  slug: foundational-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-monitors-api-openapi.yml
- filename: foundational-onboarding-api-openapi.yml
  format: yaml
  label: Foundational Onboarding API
  slug: foundational-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-onboarding-api-openapi.yml
- filename: foundational-policies-api-openapi.yml
  format: yaml
  label: Foundational Policies API
  slug: foundational-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foundational/openapi/foundational-policies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foundational.io
  spf: true
hosts:
- cert_expires: Jan  9 06:07:31 2027 GMT
  host: www.foundational.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foundational Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foundational, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foundational
provider_slug: foundational
slug: foundational-domain-security
source_filename: foundational-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foundational.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 06:07:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foundational.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/foundational/security/foundational-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Governance
- AI
- Data Management
- Lineage
---
