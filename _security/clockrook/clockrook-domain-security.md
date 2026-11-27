---
api_specs:
- filename: clockrook-account-api-openapi.yml
  format: yaml
  label: Clockrook Account API
  slug: clockrook-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-account-api-openapi.yml
- filename: clockrook-accounts-api-openapi.yml
  format: yaml
  label: Clockrook Accounts API
  slug: clockrook-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-accounts-api-openapi.yml
- filename: clockrook-jobs-api-openapi.yml
  format: yaml
  label: Clockrook Jobs API
  slug: clockrook-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-jobs-api-openapi.yml
- filename: clockrook-pricing-api-openapi.yml
  format: yaml
  label: Clockrook Pricing API
  slug: clockrook-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-pricing-api-openapi.yml
- filename: clockrook-usage-api-openapi.yml
  format: yaml
  label: Clockrook Usage API
  slug: clockrook-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clockrook.com
  spf: true
hosts:
- cert_expires: May 30 23:42:17 2027 GMT
  host: clockrook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clockrook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clockrook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clockrook
provider_slug: clockrook
slug: clockrook-domain-security
source_filename: clockrook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clockrook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 30 23:42:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clockrook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clockrook/security/clockrook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Scheduling
- Cron
- Job
- AI Agents
- Webhook
- Uptime Monitoring
- MCP
---
