---
api_specs:
- filename: ia-asso-fr-associations-api-openapi.yml
  format: yaml
  label: IA-Asso.fr Associations API
  slug: ia-asso-fr-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ia-asso-fr/openapi/ia-asso-fr-associations-api-openapi.yml
- filename: ia-asso-fr-departements-api-openapi.yml
  format: yaml
  label: IA-Asso.fr Departements API
  slug: ia-asso-fr-departements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ia-asso-fr/openapi/ia-asso-fr-departements-api-openapi.yml
- filename: ia-asso-fr-search-api-openapi.yml
  format: yaml
  label: IA-Asso.fr Search API
  slug: ia-asso-fr-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ia-asso-fr/openapi/ia-asso-fr-search-api-openapi.yml
- filename: ia-asso-fr-stats-api-openapi.yml
  format: yaml
  label: IA-Asso.fr Stats API
  slug: ia-asso-fr-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ia-asso-fr/openapi/ia-asso-fr-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ia-asso.fr
  spf: true
hosts:
- cert_expires: Jan 10 05:48:03 2027 GMT
  host: ia-asso.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IA-Asso.fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IA-Asso.fr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: IA-Asso.fr
provider_slug: ia-asso-fr
slug: ia-asso-fr-domain-security
source_filename: ia-asso-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ia-asso.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 05:48:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ia-asso.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ia-asso-fr/security/ia-asso-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Associations
- Directory
- French
- Open Data
- MCP
---
