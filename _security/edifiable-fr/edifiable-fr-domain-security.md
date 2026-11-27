---
api_specs:
- filename: edifiable-fr-plan-api-openapi.yml
  format: yaml
  label: Edifiable Plan API
  slug: edifiable-fr-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edifiable-fr/openapi/edifiable-fr-plan-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edifiable.fr
  spf: true
hosts:
- cert_expires: Jan 31 12:39:25 2027 GMT
  host: edifiable.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Edifiable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edifiable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Edifiable
provider_slug: edifiable-fr
slug: edifiable-fr-domain-security
source_filename: edifiable-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edifiable.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 12:39:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: edifiable.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/edifiable-fr/security/edifiable-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Urban Planning
- Zoning
- France
- Open Data
---
