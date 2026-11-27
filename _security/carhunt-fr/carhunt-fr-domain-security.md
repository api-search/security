---
api_specs:
- filename: carhunt-fr-analyses-api-openapi.yml
  format: yaml
  label: CarHunt Analyses API
  slug: carhunt-fr-analyses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-analyses-api-openapi.yml
- filename: carhunt-fr-compte-api-openapi.yml
  format: yaml
  label: CarHunt Compte API
  slug: carhunt-fr-compte-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-compte-api-openapi.yml
- filename: carhunt-fr-march-api-openapi.yml
  format: yaml
  label: CarHunt Marché API
  slug: carhunt-fr-march-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-march-api-openapi.yml
- filename: carhunt-fr-recherche-api-openapi.yml
  format: yaml
  label: CarHunt Recherche API
  slug: carhunt-fr-recherche-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-recherche-api-openapi.yml
- filename: carhunt-fr-synchronisation-api-openapi.yml
  format: yaml
  label: CarHunt Synchronisation API
  slug: carhunt-fr-synchronisation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-synchronisation-api-openapi.yml
- filename: carhunt-fr-watchlists-api-openapi.yml
  format: yaml
  label: CarHunt Watchlists API
  slug: carhunt-fr-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-watchlists-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carhunt.fr
  spf: true
hosts:
- cert_expires: Jan 27 19:46:49 2027 GMT
  host: carhunt.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CarHunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarHunt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CarHunt
provider_slug: carhunt-fr
slug: carhunt-fr-domain-security
source_filename: carhunt-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carhunt.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 19:46:49 2027 GMT\n  hsts: false\ndomains:\n- domain: carhunt.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/carhunt-fr/security/carhunt-fr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
