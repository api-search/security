---
api_specs:
- filename: alma-food-discovery-api-openapi.yml
  format: yaml
  label: Alma Discovery API
  slug: alma-food-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alma-food/openapi/alma-food-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alma.food
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: alma.food
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alma Food Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alma
provider_slug: alma-food
slug: alma-food-domain-security
source_filename: alma-food-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alma.food\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: alma.food\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/alma-food/security/alma-food-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Nutrition
- Artificial Intelligence
- Health
- Food Tracking
- Personalization
- Company
---
