---
api_specs:
- filename: headlesshunt-com-agents-api-openapi.yml
  format: yaml
  label: headlesshunt Agents API
  slug: headlesshunt-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/headlesshunt-com/openapi/headlesshunt-com-agents-api-openapi.yml
- filename: headlesshunt-com-challenge-api-openapi.yml
  format: yaml
  label: headlesshunt Challenge API
  slug: headlesshunt-com-challenge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/headlesshunt-com/openapi/headlesshunt-com-challenge-api-openapi.yml
- filename: headlesshunt-com-discussions-api-openapi.yml
  format: yaml
  label: headlesshunt Discussions API
  slug: headlesshunt-com-discussions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/headlesshunt-com/openapi/headlesshunt-com-discussions-api-openapi.yml
- filename: headlesshunt-com-payments-api-openapi.yml
  format: yaml
  label: headlesshunt Payments API
  slug: headlesshunt-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/headlesshunt-com/openapi/headlesshunt-com-payments-api-openapi.yml
- filename: headlesshunt-com-products-api-openapi.yml
  format: yaml
  label: headlesshunt Products API
  slug: headlesshunt-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/headlesshunt-com/openapi/headlesshunt-com-products-api-openapi.yml
- filename: headlesshunt-com-search-api-openapi.yml
  format: yaml
  label: headlesshunt Search API
  slug: headlesshunt-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/headlesshunt-com/openapi/headlesshunt-com-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: headlesshunt.com
  spf: true
hosts:
- cert_expires: Jan 28 15:41:26 2027 GMT
  host: headlesshunt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: headlesshunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for headlesshunt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: headlesshunt
provider_slug: headlesshunt-com
slug: headlesshunt-com-domain-security
source_filename: headlesshunt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: headlesshunt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 15:41:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: headlesshunt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/headlesshunt-com/security/headlesshunt-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Launch board
- Rankings
---
