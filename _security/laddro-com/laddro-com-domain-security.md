---
api_specs:
- filename: laddro-com-cover-letters-api-openapi.yml
  format: yaml
  label: Laddro Cover Letters API
  slug: laddro-com-cover-letters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laddro-com/openapi/laddro-com-cover-letters-api-openapi.yml
- filename: laddro-com-export-api-openapi.yml
  format: yaml
  label: Laddro Export API
  slug: laddro-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laddro-com/openapi/laddro-com-export-api-openapi.yml
- filename: laddro-com-resumes-api-openapi.yml
  format: yaml
  label: Laddro Resumes API
  slug: laddro-com-resumes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laddro-com/openapi/laddro-com-resumes-api-openapi.yml
- filename: laddro-com-tailor-api-openapi.yml
  format: yaml
  label: Laddro Tailor API
  slug: laddro-com-tailor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laddro-com/openapi/laddro-com-tailor-api-openapi.yml
- filename: laddro-com-templates-api-openapi.yml
  format: yaml
  label: Laddro Templates API
  slug: laddro-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laddro-com/openapi/laddro-com-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: laddro.com
  spf: true
hosts:
- cert_expires: Jan 28 18:46:23 2027 GMT
  host: laddro.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laddro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laddro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Laddro
provider_slug: laddro-com
slug: laddro-com-domain-security
source_filename: laddro-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laddro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 18:46:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: laddro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/laddro-com/security/laddro-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Resume Builder
- Career Toolkit
- Artificial Intelligence
- GDPR
- Free
- Paid Plans
---
