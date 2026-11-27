---
api_specs:
- filename: auregistre-fr-company-api-openapi.yml
  format: yaml
  label: Auregistre Company API
  slug: auregistre-fr-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auregistre-fr/openapi/auregistre-fr-company-api-openapi.yml
- filename: auregistre-fr-insolvency-api-openapi.yml
  format: yaml
  label: Auregistre Insolvency API
  slug: auregistre-fr-insolvency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auregistre-fr/openapi/auregistre-fr-insolvency-api-openapi.yml
- filename: auregistre-fr-watch-api-openapi.yml
  format: yaml
  label: Auregistre Watch API
  slug: auregistre-fr-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auregistre-fr/openapi/auregistre-fr-watch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auregistre.fr
  spf: true
hosts:
- cert_expires: Jan 15 00:09:45 2027 GMT
  host: auregistre.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auregistre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auregistre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Auregistre
provider_slug: auregistre-fr
slug: auregistre-fr-domain-security
source_filename: auregistre-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auregistre.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 00:09:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: auregistre.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/auregistre-fr/security/auregistre-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- French
- Registry
- Historical
---
