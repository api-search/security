---
api_specs:
- filename: obsidianri-com-enforcement-api-openapi.yml
  format: yaml
  label: Obsidian Enforcement API
  slug: obsidianri-com-enforcement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-enforcement-api-openapi.yml
- filename: obsidianri-com-health-api-openapi.yml
  format: yaml
  label: Obsidian Health API
  slug: obsidianri-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-health-api-openapi.yml
- filename: obsidianri-com-monitoring-api-openapi.yml
  format: yaml
  label: Obsidian Monitoring API
  slug: obsidianri-com-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-monitoring-api-openapi.yml
- filename: obsidianri-com-news-api-openapi.yml
  format: yaml
  label: Obsidian News API
  slug: obsidianri-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-news-api-openapi.yml
- filename: obsidianri-com-reference-api-openapi.yml
  format: yaml
  label: Obsidian Reference API
  slug: obsidianri-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-reference-api-openapi.yml
- filename: obsidianri-com-regulatory-api-openapi.yml
  format: yaml
  label: Obsidian Regulatory API
  slug: obsidianri-com-regulatory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-regulatory-api-openapi.yml
- filename: obsidianri-com-standards-api-openapi.yml
  format: yaml
  label: Obsidian Standards API
  slug: obsidianri-com-standards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obsidianri-com/openapi/obsidianri-com-standards-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: obsidianri.com
  spf: true
hosts:
- cert_expires: Jan 22 14:22:23 2027 GMT
  host: obsidianri.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Obsidian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obsidian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Obsidian
provider_slug: obsidianri-com
slug: obsidianri-com-domain-security
source_filename: obsidianri-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obsidianri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 14:22:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: obsidianri.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/obsidianri-com/security/obsidianri-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Regulatory
- Intelligence
- Compliance
- Monitoring
- Mapping
---
