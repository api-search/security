---
api_specs:
- filename: synergieloc-fr-acquisition-api-openapi.yml
  format: yaml
  label: Synergieloc Acquisition API
  slug: synergieloc-fr-acquisition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synergieloc-fr/openapi/synergieloc-fr-acquisition-api-openapi.yml
- filename: synergieloc-fr-api-ia-api-openapi.yml
  format: yaml
  label: Synergieloc API Ia API
  slug: synergieloc-fr-api-ia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synergieloc-fr/openapi/synergieloc-fr-api-ia-api-openapi.yml
- filename: synergieloc-fr-api-ia-industrial-api-openapi.yml
  format: yaml
  label: Synergieloc API Ia Industrial API
  slug: synergieloc-fr-api-ia-industrial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synergieloc-fr/openapi/synergieloc-fr-api-ia-industrial-api-openapi.yml
- filename: synergieloc-fr-cao-indus-api-openapi.yml
  format: yaml
  label: Synergieloc Cao Indus API
  slug: synergieloc-fr-cao-indus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synergieloc-fr/openapi/synergieloc-fr-cao-indus-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: synergieloc.fr
  spf: true
hosts:
- cert_expires: Feb 17 14:21:48 2027 GMT
  host: synergieloc.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synergieloc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synergieloc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synergieloc
provider_slug: synergieloc-fr
slug: synergieloc-fr-domain-security
source_filename: synergieloc-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synergieloc.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 14:21:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: synergieloc.fr\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/synergieloc-fr/security/synergieloc-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- RealEstate
- SaaS
- PropertyManagement
- Rental
---
