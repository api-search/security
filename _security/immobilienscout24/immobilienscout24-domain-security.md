---
api_specs:
- filename: immobilienscout24-openapi-generated.yml
  format: yaml
  label: ImmobilienScout24 API
  slug: immobilienscout24-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immobilienscout24/openapi/_ae-authored/immobilienscout24-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: immobilienscout24.de
  spf: true
hosts:
- cert_expires: May  4 23:59:59 2027 GMT
  host: www.immobilienscout24.de
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  9 23:59:59 2027 GMT
  host: api.immobilienscout24.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: rest.immobilienscout24.de
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Immobilienscout24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImmobilienScout24, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ImmobilienScout24
provider_slug: immobilienscout24
slug: immobilienscout24-domain-security
source_filename: immobilienscout24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.immobilienscout24.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  4 23:59:59 2027 GMT\n  hsts: null\n- host: api.immobilienscout24.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  9 23:59:59 2027 GMT\n  hsts: false\n- host: rest.immobilienscout24.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: immobilienscout24.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/immobilienscout24/security/immobilienscout24-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Marketplace
- API
- Germany
- Property Listings
- OAuth
- Search
- Construction Financing
---
