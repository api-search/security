---
api_specs:
- filename: free-cocktail-api-openapi.yml
  format: yaml
  label: Free Cocktail API
  slug: free-cocktail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-cocktail-api/refs/heads/main/openapi/free-cocktail-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thecocktaildb.com
  spf: false
hosts:
- cert_expires: Aug 31 02:18:02 2026 GMT
  host: www.thecocktaildb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Free Cocktail Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Free Cocktail API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Free Cocktail API
provider_slug: free-cocktail-api
slug: free-cocktail-api-domain-security
source_filename: free-cocktail-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thecocktaildb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 02:18:02 2026 GMT\n  hsts: false\ndomains:\n- domain: thecocktaildb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/free-cocktail-api/refs/heads/main/security/free-cocktail-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Beverages
- Cocktails
- Drinks
- Ingredients
- Recipes
---
