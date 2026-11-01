---
api_specs:
- filename: hortosapp-com-quote-api-openapi.yml
  format: yaml
  label: hortosapp-com Quote API
  slug: hortosapp-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hortosapp-com/openapi/hortosapp-com-quote-api-openapi.yml
- filename: hortosapp-com-search-api-openapi.yml
  format: yaml
  label: hortosapp-com Search API
  slug: hortosapp-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hortosapp-com/openapi/hortosapp-com-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hortosapp.com
  spf: true
hosts:
- cert_expires: Jan 25 18:35:41 2027 GMT
  host: hortosapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hortosapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hortosapp-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: hortosapp-com
provider_slug: hortosapp-com
slug: hortosapp-com-domain-security
source_filename: hortosapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hortosapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 18:35:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hortosapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hortosapp-com/security/hortosapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Horticulture
- Marketplace
- Wholesale
- PlantData
---
