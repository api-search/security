---
api_specs:
- filename: roboto-discovery-api-openapi.yml
  format: yaml
  label: Roboto Discovery API
  slug: roboto-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-discovery-api-openapi.yml
- filename: roboto-markdown-api-openapi.yml
  format: yaml
  label: Roboto Markdown API
  slug: roboto-markdown-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-markdown-api-openapi.yml
- filename: roboto-navigation-api-openapi.yml
  format: yaml
  label: Roboto Navigation API
  slug: roboto-navigation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-navigation-api-openapi.yml
- filename: roboto-pages-api-openapi.yml
  format: yaml
  label: Roboto Pages API
  slug: roboto-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-pages-api-openapi.yml
- filename: roboto-search-api-openapi.yml
  format: yaml
  label: Roboto Search API
  slug: roboto-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: roboto.ai
  spf: true
hosts:
- cert_expires: Dec 21 05:25:38 2026 GMT
  host: www.roboto.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Roboto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roboto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Roboto
provider_slug: roboto
slug: roboto-domain-security
source_filename: roboto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roboto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 05:25:38 2026 GMT\n  hsts: false\ndomains:\n- domain: roboto.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/roboto/security/roboto-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Robotics
- AI
- Analytics
- Platform
---
