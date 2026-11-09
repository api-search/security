---
api_specs:
- filename: basile-cc-enrichissement-api-openapi.yml
  format: yaml
  label: Basile Enrichissement API
  slug: basile-cc-enrichissement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-enrichissement-api-openapi.yml
- filename: basile-cc-entreprises-api-openapi.yml
  format: yaml
  label: Basile Entreprises API
  slug: basile-cc-entreprises-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-entreprises-api-openapi.yml
- filename: basile-cc-personnes-api-openapi.yml
  format: yaml
  label: Basile Personnes API
  slug: basile-cc-personnes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-personnes-api-openapi.yml
- filename: basile-cc-suggestions-api-openapi.yml
  format: yaml
  label: Basile Suggestions API
  slug: basile-cc-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-suggestions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: basile.cc
  spf: true
hosts:
- cert_expires: Jan 30 03:55:20 2027 GMT
  host: basile.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Basile Cc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Basile
provider_slug: basile-cc
slug: basile-cc-domain-security
source_filename: basile-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basile.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 03:55:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: basile.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/basile-cc/security/basile-cc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- B2B
- Data
- Leads
- French
- Software-as-a-Service
---
