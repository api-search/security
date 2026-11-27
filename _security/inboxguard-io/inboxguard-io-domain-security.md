---
api_specs:
- filename: inboxguard-io-account-api-openapi.yml
  format: yaml
  label: InboxGuard Account API
  slug: inboxguard-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-account-api-openapi.yml
- filename: inboxguard-io-alerts-api-openapi.yml
  format: yaml
  label: InboxGuard Alerts API
  slug: inboxguard-io-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-alerts-api-openapi.yml
- filename: inboxguard-io-domains-api-openapi.yml
  format: yaml
  label: InboxGuard Domains API
  slug: inboxguard-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-domains-api-openapi.yml
- filename: inboxguard-io-integrations-api-openapi.yml
  format: yaml
  label: InboxGuard Integrations API
  slug: inboxguard-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-integrations-api-openapi.yml
- filename: inboxguard-io-portfolio-api-openapi.yml
  format: yaml
  label: InboxGuard Portfolio API
  slug: inboxguard-io-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-portfolio-api-openapi.yml
- filename: inboxguard-io-reports-api-openapi.yml
  format: yaml
  label: InboxGuard Reports API
  slug: inboxguard-io-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-reports-api-openapi.yml
- filename: inboxguard-io-scanning-api-openapi.yml
  format: yaml
  label: InboxGuard Scanning API
  slug: inboxguard-io-scanning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-scanning-api-openapi.yml
- filename: inboxguard-io-system-api-openapi.yml
  format: yaml
  label: InboxGuard System API
  slug: inboxguard-io-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-system-api-openapi.yml
- filename: inboxguard-io-webhooks-api-openapi.yml
  format: yaml
  label: InboxGuard Webhooks API
  slug: inboxguard-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inboxguard.io
  spf: true
hosts:
- cert_expires: Apr 14 23:59:59 2027 GMT
  host: inboxguard.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InboxGuard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InboxGuard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InboxGuard
provider_slug: inboxguard-io
slug: inboxguard-io-domain-security
source_filename: inboxguard-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inboxguard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inboxguard.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inboxguard-io/security/inboxguard-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Deliverability
- DMARC
- DNS Monitoring
- Authentication
- Security
---
