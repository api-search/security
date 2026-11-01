---
api_specs:
- filename: drconsulta2-autentica-o-api-openapi.yml
  format: yaml
  label: Drconsulta2 Autenticação API
  slug: drconsulta2-autentica-o-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drconsulta2/openapi/drconsulta2-autentica-o-api-openapi.yml
- filename: drconsulta2-oracle-api-openapi.yml
  format: yaml
  label: Drconsulta2 Oracle API
  slug: drconsulta2-oracle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drconsulta2/openapi/drconsulta2-oracle-api-openapi.yml
- filename: drconsulta2-s2-api-openapi.yml
  format: yaml
  label: Drconsulta2 S2 API
  slug: drconsulta2-s2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drconsulta2/openapi/drconsulta2-s2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drconsulta.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: drconsulta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Drconsulta2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drconsulta2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Drconsulta2
provider_slug: drconsulta2
slug: drconsulta2-domain-security
source_filename: drconsulta2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drconsulta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: drconsulta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/drconsulta2/security/drconsulta2-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
