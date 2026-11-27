---
api_specs:
- filename: listar-fr-api-keys-api-openapi.yml
  format: yaml
  label: Listar API Keys API
  slug: listar-fr-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-api-keys-api-openapi.yml
- filename: listar-fr-company-enrichment-api-openapi.yml
  format: yaml
  label: Listar Company Enrichment API
  slug: listar-fr-company-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-company-enrichment-api-openapi.yml
- filename: listar-fr-company-search-api-openapi.yml
  format: yaml
  label: Listar Company Search API
  slug: listar-fr-company-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-company-search-api-openapi.yml
- filename: listar-fr-credit-api-openapi.yml
  format: yaml
  label: Listar Credit API
  slug: listar-fr-credit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-credit-api-openapi.yml
- filename: listar-fr-people-search-api-openapi.yml
  format: yaml
  label: Listar People Search API
  slug: listar-fr-people-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-people-search-api-openapi.yml
- filename: listar-fr-person-enrichment-api-openapi.yml
  format: yaml
  label: Listar Person Enrichment API
  slug: listar-fr-person-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-person-enrichment-api-openapi.yml
- filename: listar-fr-webhooks-api-openapi.yml
  format: yaml
  label: Listar Webhooks API
  slug: listar-fr-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: listar.fr
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: listar.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Listar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Listar
provider_slug: listar-fr
slug: listar-fr-domain-security
source_filename: listar-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listar.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: listar.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/listar-fr/security/listar-fr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- B2B
- Data Enrichment
- Sales
- Marketing
- Data
---
