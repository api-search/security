---
api_specs:
- filename: fieldrobin-com-agent-commerce-api-openapi.yml
  format: yaml
  label: FieldRobin Agent Commerce API
  slug: fieldrobin-com-agent-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fieldrobin-com/openapi/fieldrobin-com-agent-commerce-api-openapi.yml
- filename: fieldrobin-com-public-api-openapi.yml
  format: yaml
  label: FieldRobin Public API
  slug: fieldrobin-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fieldrobin-com/openapi/fieldrobin-com-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fieldrobin.com
  spf: true
hosts:
- cert_expires: Feb  2 00:52:28 2027 GMT
  host: fieldrobin.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FieldRobin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FieldRobin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FieldRobin
provider_slug: fieldrobin-com
slug: fieldrobin-com-domain-security
source_filename: fieldrobin-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fieldrobin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 00:52:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fieldrobin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fieldrobin-com/security/fieldrobin-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Field Service Management
- Artificial Intelligence
- Automation
- Scheduling
- Invoicing
---
