---
api_specs:
- filename: coldrig-dev-account-api-openapi.yml
  format: yaml
  label: Coldrig Account API
  slug: coldrig-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-account-api-openapi.yml
- filename: coldrig-dev-bootstrap-api-openapi.yml
  format: yaml
  label: Coldrig Bootstrap API
  slug: coldrig-dev-bootstrap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-bootstrap-api-openapi.yml
- filename: coldrig-dev-byo-domains-api-openapi.yml
  format: yaml
  label: Coldrig Byo Domains API
  slug: coldrig-dev-byo-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-byo-domains-api-openapi.yml
- filename: coldrig-dev-campaigns-api-openapi.yml
  format: yaml
  label: Coldrig Campaigns API
  slug: coldrig-dev-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-campaigns-api-openapi.yml
- filename: coldrig-dev-compliance-api-openapi.yml
  format: yaml
  label: Coldrig Compliance API
  slug: coldrig-dev-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-compliance-api-openapi.yml
- filename: coldrig-dev-dashboard-api-openapi.yml
  format: yaml
  label: Coldrig Dashboard API
  slug: coldrig-dev-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-dashboard-api-openapi.yml
- filename: coldrig-dev-inbox-api-openapi.yml
  format: yaml
  label: Coldrig Inbox API
  slug: coldrig-dev-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-inbox-api-openapi.yml
- filename: coldrig-dev-infrastructure-api-openapi.yml
  format: yaml
  label: Coldrig Infrastructure API
  slug: coldrig-dev-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-infrastructure-api-openapi.yml
- filename: coldrig-dev-leads-api-openapi.yml
  format: yaml
  label: Coldrig Leads API
  slug: coldrig-dev-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-leads-api-openapi.yml
- filename: coldrig-dev-messages-api-openapi.yml
  format: yaml
  label: Coldrig Messages API
  slug: coldrig-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-messages-api-openapi.yml
- filename: coldrig-dev-sandbox-api-openapi.yml
  format: yaml
  label: Coldrig Sandbox API
  slug: coldrig-dev-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-sandbox-api-openapi.yml
- filename: coldrig-dev-webhooks-api-openapi.yml
  format: yaml
  label: Coldrig Webhooks API
  slug: coldrig-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coldrig.dev
  spf: true
hosts:
- cert_expires: Dec 10 15:16:47 2026 GMT
  host: coldrig.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coldrig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coldrig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coldrig
provider_slug: coldrig-dev
slug: coldrig-dev-domain-security
source_filename: coldrig-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coldrig.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 15:16:47 2026 GMT\n  hsts: false\ndomains:\n- domain: coldrig.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/coldrig-dev/security/coldrig-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cold Email
- Outreach
- AI Agents
- Email Infrastructure
---
