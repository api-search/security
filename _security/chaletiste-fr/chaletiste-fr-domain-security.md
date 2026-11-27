---
api_specs:
- filename: chaletiste-fr-calculs-api-openapi.yml
  format: yaml
  label: Chaletiste Calculs API
  slug: chaletiste-fr-calculs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaletiste-fr/openapi/chaletiste-fr-calculs-api-openapi.yml
- filename: chaletiste-fr-donn-es-api-openapi.yml
  format: yaml
  label: Chaletiste Données API
  slug: chaletiste-fr-donn-es-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaletiste-fr/openapi/chaletiste-fr-donn-es-api-openapi.yml
- filename: chaletiste-fr-recherche-api-openapi.yml
  format: yaml
  label: Chaletiste Recherche API
  slug: chaletiste-fr-recherche-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaletiste-fr/openapi/chaletiste-fr-recherche-api-openapi.yml
- filename: chaletiste-fr-transactions-api-openapi.yml
  format: yaml
  label: Chaletiste Transactions API
  slug: chaletiste-fr-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaletiste-fr/openapi/chaletiste-fr-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chaletiste.fr
  spf: true
hosts:
- cert_expires: Dec 25 16:16:46 2026 GMT
  host: chaletiste.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chaletiste Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chaletiste, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chaletiste
provider_slug: chaletiste-fr
slug: chaletiste-fr-domain-security
source_filename: chaletiste-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaletiste.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 16:16:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chaletiste.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chaletiste-fr/security/chaletiste-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Real Estate
- Construction
- Open Data
---
