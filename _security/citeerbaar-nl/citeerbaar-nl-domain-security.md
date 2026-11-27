---
api_specs:
- filename: citeerbaar-nl-agents-api-openapi.yml
  format: yaml
  label: Citeerbaar Agents API
  slug: citeerbaar-nl-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeerbaar-nl/openapi/citeerbaar-nl-agents-api-openapi.yml
- filename: citeerbaar-nl-open-data-api-openapi.yml
  format: yaml
  label: Citeerbaar Open data API
  slug: citeerbaar-nl-open-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeerbaar-nl/openapi/citeerbaar-nl-open-data-api-openapi.yml
- filename: citeerbaar-nl-status-api-openapi.yml
  format: yaml
  label: Citeerbaar Status API
  slug: citeerbaar-nl-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeerbaar-nl/openapi/citeerbaar-nl-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: citeerbaar.nl
  spf: true
hosts:
- cert_expires: May  4 23:59:59 2027 GMT
  host: citeerbaar.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Citeerbaar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citeerbaar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Citeerbaar
provider_slug: citeerbaar-nl
slug: citeerbaar-nl-domain-security
source_filename: citeerbaar-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citeerbaar.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: citeerbaar.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/citeerbaar-nl/security/citeerbaar-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- SEO
- Digital-PR
- Netherlands
- Citations
---
