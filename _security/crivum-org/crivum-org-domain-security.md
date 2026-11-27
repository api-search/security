---
api_specs:
- filename: crivum-org-avaliacoes-api-openapi.yml
  format: yaml
  label: Crivum Avaliacoes API
  slug: crivum-org-avaliacoes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-avaliacoes-api-openapi.yml
- filename: crivum-org-criterios-api-openapi.yml
  format: yaml
  label: Crivum Criterios API
  slug: crivum-org-criterios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-criterios-api-openapi.yml
- filename: crivum-org-records-api-openapi.yml
  format: yaml
  label: Crivum Records API
  slug: crivum-org-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-records-api-openapi.yml
- filename: crivum-org-saldo-api-openapi.yml
  format: yaml
  label: Crivum Saldo API
  slug: crivum-org-saldo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-saldo-api-openapi.yml
- filename: crivum-org-triagem-api-openapi.yml
  format: yaml
  label: Crivum Triagem API
  slug: crivum-org-triagem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-triagem-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crivum.org
  spf: true
hosts:
- cert_expires: Jan 20 22:40:38 2027 GMT
  host: crivum.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crivum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crivum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crivum
provider_slug: crivum-org
slug: crivum-org-domain-security
source_filename: crivum-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crivum.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 22:40:38 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crivum.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crivum-org/security/crivum-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Platform
- Evaluation
- Publishing
- Artificial Intelligence
- Portuguese
---
