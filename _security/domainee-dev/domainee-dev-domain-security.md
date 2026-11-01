---
api_specs:
- filename: domainee-dev-dns-api-openapi.yml
  format: yaml
  label: domainee-dev DNS API
  slug: domainee-dev-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-dns-api-openapi.yml
- filename: domainee-dev-domain-purchases-api-openapi.yml
  format: yaml
  label: domainee-dev Domain purchases API
  slug: domainee-dev-domain-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-domain-purchases-api-openapi.yml
- filename: domainee-dev-domains-api-openapi.yml
  format: yaml
  label: domainee-dev Domains API
  slug: domainee-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-domains-api-openapi.yml
- filename: domainee-dev-free-tools-api-openapi.yml
  format: yaml
  label: domainee-dev Free tools API
  slug: domainee-dev-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-free-tools-api-openapi.yml
- filename: domainee-dev-origin-secret-api-openapi.yml
  format: yaml
  label: domainee-dev Origin secret API
  slug: domainee-dev-origin-secret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-origin-secret-api-openapi.yml
- filename: domainee-dev-projects-api-openapi.yml
  format: yaml
  label: domainee-dev Projects API
  slug: domainee-dev-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-projects-api-openapi.yml
- filename: domainee-dev-service-api-openapi.yml
  format: yaml
  label: domainee-dev Service API
  slug: domainee-dev-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-service-api-openapi.yml
- filename: domainee-dev-webhooks-api-openapi.yml
  format: yaml
  label: domainee-dev Webhooks API
  slug: domainee-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: domainee.dev
  spf: true
hosts:
- cert_expires: May  7 23:59:59 2027 GMT
  host: domainee.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domainee Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for domainee-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: domainee-dev
provider_slug: domainee-dev
slug: domainee-dev-domain-security
source_filename: domainee-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domainee.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: domainee.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/domainee-dev/security/domainee-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API
- SaaS
- Custom-Domains
- Free-Tier
- MCP
---
