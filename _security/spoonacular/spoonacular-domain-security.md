---
api_specs:
- filename: spoonacular-openapi.yml
  format: yaml
  label: Spoonacular
  slug: spoonacular
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/openapi/spoonacular-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: spoonacular.com
  spf: true
hosts:
- cert_expires: Sep 19 20:31:07 2026 GMT
  host: spoonacular.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 20:31:07 2026 GMT
  host: api.spoonacular.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spoonacular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spoonacular, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Spoonacular
provider_slug: spoonacular
slug: spoonacular-domain-security
source_filename: spoonacular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spoonacular.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:31:07 2026 GMT\n  hsts: false\n- host: api.spoonacular.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:31:07 2026 GMT\n  hsts: null\ndomains:\n- domain: spoonacular.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/security/spoonacular-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Restaurant
- Food And Drink
- Recipes
- Nutrition
- Meal Planning
- Public APIs
---
