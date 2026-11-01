---
api_specs:
- filename: superglue-connections-api-openapi.yml
  format: yaml
  label: Index Commerce Connections API
  slug: superglue-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superglue/openapi/superglue-connections-api-openapi.yml
- filename: superglue-runs-api-openapi.yml
  format: yaml
  label: Index Commerce Runs API
  slug: superglue-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superglue/openapi/superglue-runs-api-openapi.yml
- filename: superglue-tools-api-openapi.yml
  format: yaml
  label: Index Commerce Tools API
  slug: superglue-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superglue/openapi/superglue-tools-api-openapi.yml
- filename: superglue-webhooks-api-openapi.yml
  format: yaml
  label: Index Commerce Webhooks API
  slug: superglue-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superglue/openapi/superglue-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: superglue.ai
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: superglue.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Superglue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Index Commerce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Index Commerce
provider_slug: superglue
slug: superglue-domain-security
source_filename: superglue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superglue.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: superglue.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/superglue/security/superglue-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Platform
- Storefront
- Analytics
---
