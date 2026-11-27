---
api_specs:
- filename: symphony-fr-baskets-api-openapi.yml
  format: yaml
  label: Symphony Baskets API
  slug: symphony-fr-baskets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symphony-fr/openapi/symphony-fr-baskets-api-openapi.yml
- filename: symphony-fr-ingredients-api-openapi.yml
  format: yaml
  label: Symphony Ingredients API
  slug: symphony-fr-ingredients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symphony-fr/openapi/symphony-fr-ingredients-api-openapi.yml
- filename: symphony-fr-recipes-api-openapi.yml
  format: yaml
  label: Symphony Recipes API
  slug: symphony-fr-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symphony-fr/openapi/symphony-fr-recipes-api-openapi.yml
- filename: symphony-fr-users-api-openapi.yml
  format: yaml
  label: Symphony Users API
  slug: symphony-fr-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symphony-fr/openapi/symphony-fr-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: true
  domain: symphony.fr
  spf: true
hosts:
- cert_expires: Jan 24 20:27:51 2027 GMT
  host: symphony.fr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Symphony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symphony, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Symphony
provider_slug: symphony-fr
slug: symphony-fr-domain-security
source_filename: symphony-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: symphony.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 20:27:51 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: symphony.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/symphony-fr/security/symphony-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Meal Delivery
- Nutrition
- Personalized Meals
- French Startup
- Health Tech
---
